<img src="https://github.com/marihere/subliminally/blob/main/images/banner.png">

#

<p align="center">Subliminally is a program designed to make creating subliminal audios as easy as possible.</p>
<br>

## Table of contents
1. [Introduction](https://github.com/marihere/subliminally#introduction)
2. [Getting started](https://github.com/marihere/subliminally#getting-started)
3. [Donate](https://github.com/marihere/subliminally_gui#donate)
4. [Usage](https://github.com/marihere/subliminally_gui#usage)
5. [Example](https://github.com/marihere/subliminally#example)
6. [Unlicense](https://github.com/marihere/subliminally#unlicense)

<br>

## Introduction

Subliminally is program  written with Python designed to make creating subliminal audios as easy as possible.


### How does it work?

Subliminally requests four different inputs: the main affirmations, the booster affirmations, an image file, and an audio file (e.g. a song of choice). <br>
These four inputs are then elaborated using a pretty simple algorithm. Here a pretty simplified version of the main algorithm:
<br>

<img src="https://github.com/marihere/subliminally/blob/main/images/algorithm.png">

<br>

The algorithm behind the creation of the subliminal audio is the most important one. Here it is:

<img src="https://github.com/marihere/subliminally/blob/main/images/algorithm_subaudio.png">
<br>
<i>affs is the affirmations audio file; bg is the background audio file; affs_length and bg_length are the duration (in seconds) of the respective audio files.</i>

<br>

## Getting started

Subliminally has two different versions:
- the <b>graphical user interface</b> (GUI) version;
- the <b>command line interface</b> (CLI) version.

Let's see the differences between the two:
| CLI | GUI |
|:---:|:---:|
| Maybe harder to use for beginners. | It is generally easier to use. |
| It is faster. | It is much slower. |
| Affirmations must be written in a file, before running the script. | Affirmations can be written while the program is running. |

### Installation

#### CLI version

```console
$ git clone https://github.com/marihere/subliminally
$ cd subliminally
$ python .\lib\main.py
```

#### GUI version

The GUI version can be found [here](https://github.com/marihere/subliminally_gui).

<br>

## Donate

<a href="https://paypal.me/mariminnie/"><img src="blue.svg" height="40"></a>  

<br>

## Usage

```console
$ python .\lib\main.py --help
usage: main.py [-h] -t TITLE -a AFFS -b BG -i IMG

Subliminally: Create Subliminals Easily

optional arguments:
  -h, --help            show this help message and exit
  -t TITLE, --title TITLE
                        title for your subliminal
  -a AFFS, --affs AFFS  text file of the affirmations for your subliminal
  -b BG, --bg BG        audio file for your subliminal
  -i IMG, --img IMG     image file for your subliminal
```

<br>

## Example

```console
$ python .\lib\main.py --title mysubliminal --affs .\example\affirmations.txt --bg .\example\rainfall_sounds.wav --img .\example\image.jpg
```

### Result:

[Audio result](https://github.com/marihere/subliminally/blob/main/example/audios/mysubliminal.wav)

[Video result](https://github.com/marihere/subliminally/blob/main/example/videos/mysubliminal.mp4)

<br>

## Unlicense

[The Unlicense](https://github.com/marihere/subliminally/blob/main/UNLICENSE)
