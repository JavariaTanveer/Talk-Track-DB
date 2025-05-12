## TalkTrackDB
 **TalkTrackDB** is a speech-to-text pipeline that leverages the power of SpeechBrain and Wav2Vec2 to transcribe audio files and store the results in a lightweight SQLite database.

Ideal for developers, researchers, and hobbyists working on voice-driven applications or audio archiving.

---

## Features

*  **Speech-to-Text Conversion** using the Wav2Vec2 model via SpeechBrain
*  **SQLite Integration** for storing and querying transcriptions
* Easy handling of `.wav` audio files
* Extensible framework for analysis, tagging, or search

---

## Requirements

This notebook installs everything you need:

```bash
pip install speechbrain torchaudio
```

No external database needed — uses Python's built-in `sqlite3` for storage.

---

##  How to Use

1. **Upload `.wav` audio files** (preferably 16kHz mono)
2. **Run the notebook cells** to:

   * Load and process audio
   * Generate transcriptions
   * Store results in SQLite
3. **Query the database** to view or filter transcripts

---

##  Database Schema

SQLite stores the following fields:

* `id` – unique identifier
* `file_name` – original file name
* `transcription` – converted text from speech
* `timestamp` – processing time or file metadata (optional)

---

##  Powered By

* [SpeechBrain](https://speechbrain.readthedocs.io)
* [Wav2Vec2 (Facebook AI)](https://huggingface.co/facebook/wav2vec2-base-960h)
* `torchaudio`, `sqlite3`, and other Python tools

---

##  Example Use Cases

* Voice note transcription
* Audio archival and indexing
* Building search engines for podcasts or interviews
* Preprocessing for voice-based NLP tasks

---
![talk track DB](https://github.com/user-attachments/assets/8c3b8cee-2f41-46ff-8795-d8938c515295)

