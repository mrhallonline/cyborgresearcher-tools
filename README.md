# cyborgresearcher-tools

WhisperX Transcription + Diarization Audio Processing (Colab Edition)
This repository contains a Google Colab-ready Jupyter notebook for qualitative researchers to transcribe, diarize speakers, and convert audio files into usable text formats (CSV, TXT, JSON, and VTT). It combines advanced transcription capabilities from WhisperX with diarization support from pyannote.audio.

What This Version Does
✅ Runs entirely in-browser (via Google Colab)
✅ Installs all packages automatically
✅ Accepts file uploads (.wav, .mp3, .ogg) for transcription
✅ Prompts for a Hugging Face token (required for diarization)
✅ Supports speaker diarization and pseudonym replacement
✅ Saves outputs in CSV format, ready for coding or analysis

How to Use This Notebook
A. Open the Notebook in Colab
B. Upload Your Files
You’ll be prompted to upload:
Your audio file (must be .wav, .mp3, or .ogg)

(Optional) A CSV file named pseudonyms.csv to anonymize names and locations

C. Enter Hugging Face Token
This is needed specifically for speaker diarization.
If you don’t already have one, follow these steps:

Go to https://huggingface.co/settings/tokens

Click "New token"

Copy the token and paste it when prompted in the notebook

D. Outputs
The notebook will generate:

transcript_output.csv: includes start, end, text, and speaker

Word-level aligned transcripts

Anonymized output (if pseudonyms were uploaded)

Sample Files
You can try out the pipeline with these:

sample_clip.wav: A 10-second placeholder audio file

pseudonyms.csv: Example mapping of real names to pseudonyms

Example CSV Output
start	end	speaker	text
0.23	2.14	Speaker A	Yeah, I think that’s true…
2.15	3.40	Speaker B	But it depends on the context.

Notes on Privacy
All processing happens within the Colab environment. No audio or transcript files are uploaded to third-party servers (except to Whisper/pyannote models through Hugging Face). That said, please anonymize your files or use the provided pseudonym system when working with identifiable data.

Credits and Attribution
WhisperX by @m-bain

Speaker diarization models by pyannote

Notebook adaptations and educational framing by @cyborgresearcher

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mrhallonline/cyborgresearcher-tools/blob/main/whisperx_colab_edition.ipynb)
