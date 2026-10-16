---
name: openai-whisper
description: Local speech-to-text with the Whisper CLI (no API key).
homepage: https://openai.com/research/whisper
metadata:
  {
    "brigade":
      {
        "emoji": "🎤",
        "requires": { "bins": ["whisper"] },
        "install":
          [
            {
              "id": "brew",
              "kind": "manual",
              "hint": "pip install openai-whisper (or: winget install Gyan.FFmpeg / choco install ffmpeg for audio deps)",
              "bins": ["whisper"],
              "label": "Install OpenAI Whisper (pip)",
            },
          ],
      },
  }
---

# Whisper (CLI)

Use `whisper` to transcribe audio locally.

Quick start

- `whisper /path/audio.mp3 --model medium --output_format txt --output_dir .`
- `whisper /path/audio.m4a --task translate --output_format srt`

Notes

- Models download to `~/.cache/whisper` on first run.
- `--model` defaults to `turbo` on this install.
- Use smaller models for speed, larger for accuracy.
- `--task translate` outputs ENGLISH. It cannot produce Arabic or other target languages; for non-English output transcribe then translate separately.
- Never pass `--task translate` together with `--model turbo` or a `.en` model; those are English-only and the combination is meaningless.
