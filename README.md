# cyborgresearcher-tools

WhisperX + Speaker Diarization (Colab Edition)
This repository provides a Google Colab notebook for transcribing and diarizing audio files using WhisperX and pyannote.audio. The goal is to support qualitative researchers—especially in education and the social sciences—by making complex NLP tools accessible.

🔍 What This Version Does
Transcribes audio with WhisperX, including word-level timestamps

Performs speaker diarization using Hugging Face’s pyannote/speaker-diarization

Merges speaker segments with aligned transcript using timestamp overlap

Outputs a clean CSV with start, end, word, and speaker

All in a single browser session, no installation needed.

🚀 How to Use
A. Run in Colab

B. Upload Files
You’ll be prompted to upload:

An audio file (.wav, .mp3, or .ogg)

(Optional) A pseudonyms.csv file if you're integrating anonymization in a later step

C. Enter Hugging Face Token
To run the diarization step, the notebook will ask for a Hugging Face token.
👉 Get yours here

D. Output
The notebook will generate:

Column	Description
start	Start time of each word
end	End time of each word
word	Transcribed word text
speaker	Speaker label from diarization

All of this is saved as transcript_with_speakers.csv.

📂 Sample Files
Try it out with:

sample_clip.wav

pseudonyms.csv

These are especially helpful if you're new to audio transcription pipelines.

🧠 Educational Use Cases
Discourse analysis in classrooms

Coding teacher interviews for student agency

Identifying shifts in speaker stance over time

Locating affective or epistemic language by speaker

🔒 Notes on Privacy
This tool is designed with ethical research in mind. All processing occurs inside your Colab session. No audio or transcripts are uploaded to external servers beyond what's required by Hugging Face diarization models.

👋 Questions?
This tool is part of a broader effort to create accessible NLP-powered research workflows for education researchers. If you're curious, stuck, or excited, reach out or explore the other tools in this repo.


Credits and Attribution
WhisperX by @m-bain

Speaker diarization models by pyannote

Notebook adaptations and educational framing by @cyborgresearcher

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mrhallonline/cyborgresearcher-tools/blob/main/whisperx_colab_edition.ipynb)
