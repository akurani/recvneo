# recvneo - Send Receiver for AlphaSmart Neo

by Amar Kurani

* [https://github.com/akurani](https://github.com/akurani)
* [https://twitter.com/AmarKurani](https://twitter.com/AmarKurani)

## Introduction

recvneo is a simple script which receives text transmitted from an AlphaSmart
Neo via the SEND button and saves it to a UTF-8 text file.

The SEND button works by transmitting the text from the AlphaSmart to the
computer via STDIN. I.e, the AlphaSmart "types" out the file's text to the
computer.

Normally, you'll use the SEND button with a text editor or word processor. This
script is a fire-and-forget alternative.

Learn more about the AlphaSmart Neo:

[https://en.wikipedia.org/wiki/AlphaSmart](https://en.wikipedia.org/wiki/AlphaSmart)

It was designed for the classroom, but others and myself and found use as a
very focused writing tool. It's the hardware equivalent of those distraction-free
text editors like FocusWriter.

## Installation

recvneo requires Python 2.7 and only the standard libraries. Copy the script
to somewhere in your PATH and set the executable bit (i.e., chmod +x recvneo).

## Usage

1. Connect your AlphaSmart to your computer with a USB cable.
2. Run this script.
3. In your AlphaSmart, go to your text file and then press SEND.
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
along with this program.  If not, see [http://www.gnu.org/licenses/](http://www.gnu.org/licenses/).
