# 🎬 AI Music Video Agent

> **An autonomous pipeline that directs, composes, and edits seamless music videos from a single text theme.**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![Google Gemini](https://img.shields.io/badge/AI-Google%20Gemini-orange)](https://deepmind.google/technologies/gemini/)
[![Replicate](https://img.shields.io/badge/API-Replicate-black)](https://replicate.com/)

## 📖 Overview

This project implements a multi-modal AI agent that acts as a creative director. Given a simple theme (e.g., "Cyberpunk City in Rain"), it orchestrates multiple AI models to produce a complete audiovisual experience.

The pipeline includes:
1.  **The Director (Gemini 2.0):** Generates precise artistic prompts for music and video.
2.  **The Composer (MusicGen):** Creates background music matching the mood.
3.  **The Videographer (Minimax):** Generates high-quality short video clips.
4.  **The Editor (MoviePy & FFMPEG):** Automatically repairs video metadata, creates seamless loops (Ping-Pong/Crossfade), and merges audio.

## 🚀 Features

* **Prompt Engineering:** Uses Google Gemini to convert simple ideas into detailed style guides.
* **Robust Video Processing:** Includes an FFMPEG wrapper to fix corrupted headers often found in AI-generated video streams.
* **Seamless Looping:**
    * *Ping-Pong Mode:* Creates perfect loops by reversing playback (Boomerang effect).
    * *Crossfade Mode:* Traditional seamless blending.
* **Colab Ready:** Designed to run smoothly in Google Colab free tier.

## 🛠️ Tech Stack

* **Core Logic:** Python
* **LLM:** Google Gemini API
* **Generative Models:** Replicate API (Minimax for video, Meta MusicGen for audio)
* **Media Processing:** MoviePy, FFMPEG

