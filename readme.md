# recvneo - Receiver for AlphaSmart Neo

by Amar Kurani

* <https://github.com/akurani>
* <http://amarkurani.com>

## Introduction

recvneo is a script which receives text transmitted from an AlphaSmart
Neo via the SEND button and saves it to a UTF-8 text file.

The SEND button transmits text from the AlphaSmart to STDIN. I.e, the AlphaSmart 
"types" out the file's text to the computer.

Normally, you'd use the SEND button with a text editor or word processor. This
script is a fire-and-forget alternative.

Learn more about the AlphaSmart Neo:

<https://en.wikipedia.org/wiki/AlphaSmart>

The AlphaSmarts were designed for the classroom, but others and myself have
found them very good as a very focused writing tool. It's the hardware
equivalent of those distraction-free text editors like FocusWriter.

## Installation

Copy the script to somewhere in your PATH and set the executable bit:

    chmod +x recvneo

### Python 2 and 3

recvneo runs with Python 2.7.11+ or Python 3.5.1+ and the standard libraries.

## Usage

1. Connect your AlphaSmart to your computer with a USB cable.
2. On your computer, run this script.
3. On your AlphaSmart, go to your text file and then press SEND.
4. Wait until the text is fully transmitted and the script terminates.

Run "recvneo --help" to learn about the command-line options.

## Licensed under GPL v3:

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>
