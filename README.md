# LibMP

**LibMP** is a lightweight, high-performance, and memory-safe universal audio decoding and playback engine for Python, powered by Rust, FFmpeg, and Rodio. 

## Features
- **Memory-Safe Backend:** Written in Rust, preventing memory leaks and data races.
- **FFmpeg Powered:** Supports decoding for a wide variety of audio formats.
- **Rodio Audio Output:** Smooth and low-latency audio playback.
- **Playlist Management:** Built-in playlist support with track addition, removal, auto-advance, and navigation (`next`/`previous`).
- **Python 3.6+ Support:** Easy integration with Python applications using PyO3.

## Installation

You can install LibMP locally or via pip:

```bash
pip install libmp
````

## Python Code (Demo; As Example)

```python

import libmp

# Initialize the player
player = libmp.LibMP()

# Add tracks to the playlist
player.add_track("song1.mp3")
player.add_track("song2.wav")

# Start playback
player.play()

# Control volume (0.0 to 1.0)
player.set_volume(0.8)

# Check playback status
print("Current Position:", player.get_position())
print("Total Duration:", player.get_duration())

# Pause or Stop
# player.pause()
# player.stop()
```

## Licence (GNU Lesser General Public License (LGPL) v 2.1)

GNU LESSER GENERAL PUBLIC LICENSE

Version 2.1, February 1999

Copyright (C) 2026 PlayMulti46 <playmulti844@gmail.com>

This library is free software; you can redistribute it and/or modify it 
under the terms of the GNU Lesser General Public License as published by 
the Free Software Foundation; either version 2.1 of the License, or (at 
your option) any later version.

This library is distributed in the hope that it will be useful, but WITHOUT 
ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or 
FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License 
for more details.
