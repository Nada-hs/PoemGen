# PoemGen
# PoemGen: AI Poetry Generation Project

This project integrates several AI tasks, including text generation, text-to-speech, and text-to-image functionalities, using models from Hugging Face's Transformers library. The project enables the generation of text in both Arabic and English, converts text to speech in both languages, and generates images based on textual descriptions.

## Features

1. **Poem Generation**:
   - Arabic poem generation using the `akhooli/ap2023` model.
   - English poem generation using the `ashiqabdulkhader/GPT2-Poet` model.

2. **Text-to-Speech (TTS)**:
   - Converts Arabic poems to speech using the `MBZUAI/speecht5_tts_clartts_ar` model.
   - Converts English poems to speech using the `microsoft/speecht5_tts` model.

3. **Text-to-Image**:
   - Generates an image from the text of an English poem using the `CompVis/stable-diffusion-v1-4` model.
echo "# PoemGen" >> README.md
4. **Gradio Interface**:
   - An interactive web interface where users can:
     - Generate poems in Arabic or English.
     - Convert generated poems into speech (TTS).
     - Generate an image based on the poem.

## Dependencies

To run the project, the following Python packages are required:

- `transformers`
- `gradio`
- `torch`
- `uvicorn`
- `soundfile`
- `datasets`
- `diffusers`

Install these dependencies using pip:

```bash
pip install transformers gradio torch uvicorn soundfile datasets diffusers

## Funcations

1. **Poem Generation**:

- The `generate_poem` function generates a poem or text based on a provided sentence.

2. **Text-to-Speech (TTS)**:

- The `text_to_speech_arabic` function converts Arabic text to speech.
- The `text_to_speech_english` function converts English text to speech.

4. **Gradio Interface**:
- The `generate_image_from_poem` function creates an image based on the input poem.

### 4- Gradio Interface:

- The Gradio interface can be launched with `my_model.launch()`.

## Running the Project
To run the project locally, use the following steps:
    1- Clone or download the project.
    2- Install the required dependencies.
    3- Execute the script:

This will open a Gradio UI where you can select the language (Arabic or English), input a sentence, and generate the following outputs:

- A poem.
- Audio of the generated poem (TTS).
- An image based on the generated poem.

## Example Inputs

Here are some example inputs to use in the Gradio interface:

- **English**: `"The shining sun rises over the calm ocean."`
- **Arabic**: `"الورود تتفتح في الربيع"` (Translation: "The flowers bloom in spring.")

