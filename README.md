# vidtoolz-replace-audio

[![PyPI](https://img.shields.io/pypi/v/vidtoolz-replace-audio.svg)](https://pypi.org/project/vidtoolz-replace-audio/)
[![Changelog](https://img.shields.io/github/v/release/sukhbinder/vidtoolz-replace-audio?include_prereleases&label=changelog)](https://github.com/sukhbinder/vidtoolz-replace-audio/releases)
[![Tests](https://github.com/sukhbinder/vidtoolz-replace-audio/workflows/Test/badge.svg)](https://github.com/sukhbinder/vidtoolz-replace-audio/actions?query=workflow%3ATest)
[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/sukhbinder/vidtoolz-replace-audio/blob/main/LICENSE)

Replace audio for a video file

![vidtoolz-replace-audio demo](https://github.com/sukhbinder/vidtoolz-replace-audio/blob/main/vidtoolz-repaudio.gif)

## Installation

First install [vidtoolz](https://github.com/sukhbinder/vidtoolz).

```bash
pip install vidtoolz
```

Then install this plugin in the same environment as your vidtoolz application.

```bash
vidtoolz install vidtoolz-replace-audio
```
## Usage

type ``vidtoolz-replace-audio --help`` to get help


```bash
usage: vid repaudio [-h] [-o OUTPUT] [-v VOLUME] [-s STARTAT] video audio

Replace audio for a video file

positional arguments:
  video                 Path to the input video file
  audio                 Path to the audio file

optional arguments:
  -h, --help            show this help message and exit
  -o OUTPUT, --output OUTPUT
                        Path to save the output video. Default None
  -v VOLUME, --volume VOLUME
                        Percentage to lower the original audio (0-100),
                        Default 30
  -s STARTAT, --startat STARTAT
                        Load audio at this time in seconds. Default 0

```

## Development

To set up this plugin locally, first checkout the code. Then create a new virtual environment:
```bash
cd vidtoolz-replace-audio
python -m venv venv
source venv/bin/activate
```
Now install the dependencies and test dependencies:
```bash
pip install -e '.[test]'
```
To run the tests:
```bash
python -m pytest
```
