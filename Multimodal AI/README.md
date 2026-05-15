# Multimodal AI | Hack Invaders Workshop

A small Python script that turns a photo of a receipt into structured JSON using Google's Gemini API. Pass an image path, get back structured data.

Slides Link: https://docs.google.com/presentation/d/1i3tRTKLffDnHAPCFMsqDZ6ZE98VjGSvuYvPgaIT61kQ/

## What You'll Learn

- How to send images to the Gemini API
- How to prompt a vision model for structured data
- How to load API keys from a `.env` file
- How to extend the same pattern to other image-to-data tasks

## Tech Stack

- Python 3
- google-genai
- python-dotenv
- Gemini 2.5 Flash

## Local Setup

Create and activate a virtual environment so dependencies stay isolated to this project:

```sh
python3 -m venv venv
source venv/bin/activate
```

On Windows, activate with `venv\Scripts\activate` instead.

Add `venv` to your `.gitignore`. When you're done working, run `deactivate` to exit the environment.

Install the dependencies:

```sh
pip install google-genai python-dotenv
```

Create a `.env` file in the same directory as the script:

```sh
GEMINI_API_KEY=your_key_here
```

Get a key at https://aistudio.google.com/app/apikey. Add `.env` to your `.gitignore` — never commit API keys.

## Usage

Run the script with a path to a receipt image:

```sh
python receipt.py path/to/receipt.jpg
```

Example output:

```json
{
  "vendor": "Trader Joe's",
  "date": "2025-11-12",
  "items": [
    {"name": "Bananas", "price": 0.59},
    {"name": "Almond Butter", "price": 7.99}
  ],
  "total": 8.58,
  "currency": "USD"
}
```

## How It Works

The script does five things:

1. Read the image into bytes

`Path(image_path).read_bytes()` loads the file from disk.

2. Wrap the bytes for the API

`types.Part.from_bytes(data=..., mime_type="image/jpeg")` attaches the image to the request.

3. Send the image plus a prompt

The prompt names every field you want and the format for each one (date as `YYYY-MM-DD`, currency as a 3-letter code).

4. Get JSON output

`response_mime_type="application/json"` stops the model from wrapping the result in markdown fences.

5. Parse the response

`json.loads(response.text)` turns the string into a Python dict, we now have structured data we can use!
