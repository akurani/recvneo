# recvneo - Receiver for AlphaSmart Neo

by Amar Kurani

* <https://github.com/akurani>
* <http://amarkurani.com>

## Introduction

recvneo is a script which receives text transmitted from an AlphaSmart
Neo via the SEND button and saves it to a UTF-8 text file. Learn more about the 
AlphaSmart Neo: <https://en.wikipedia.org/wiki/AlphaSmart>

The SEND button transmits text from the AlphaSmart to STDIN. I.e, the AlphaSmart 
"types" out the file's text to the computer.

Normally, you'd use the SEND button with a text editor or word processor. This
script is a fire-and-forget alternative.

The AlphaSmarts were designed for the classroom, but others and myself have
found them very good as a very focused writing tool. It's the hardware
equivalent of those distraction-free text editors like FocusWriter.

## Requirements

recvneo requires Python 2.7.11+ or Python 3.5.1+ and the standard libraries.

## Installation

On Mac or Linux, copy the script to somewhere in your PATH and set the executable bit:

    chmod +x recvneo

NOTE: untested on other OSs.

## Usage

1. Connect your AlphaSmart to your computer with a USB cable.
2. On your computer, run this script.
3. On your AlphaSmart, go to your text file and then press SEND.
4. Wait until the text is fully transmitted and the script terminates.

Run "recvneo --help" to learn about the command-line options:

    usage: recvneo [-h] [-e] [-m {write,w,overwrite,o,append,a}] [-n] [-r]
                   [-t TIMEOUT] [-w]
                   [filename]

    Saves text received via an AlphaSmart Neo's 'send' function into a UTF-8 text
    file. Run this script, and then hit the 'send' button on the Neo.

    positional arguments:
      filename              Optional name of the UTF-8 text file which will store
                            the Neo text. Default = a generic name with timestamp
                            (e.g., neotext--2016-05-12--10-06-52.txt).

    optional arguments:
      -h, --help            show this help message and exit
      -e, --echo            Echos the Neo text to the console as it's received.
      -m {write,w,overwrite,o,append,a}, --mode {write,w,overwrite,o,append,a}
                            File-write mode: 'write' or 'w' to a new file (failing
                            if it already exists); 'overwrite' or 'o' an existing
                            file (creating one if it doesn't exist); 'append' or
                            'a' to an existing file (creating one if it doesn't
                            exist). Default = write.
      -n, --numbered        Appends a '-####' numerical suffix to the filename
                            where the number is one larger than what's found in
                            similiarly named files in the same directory. E.g.,
                            neotext-0001.txt, neotext-0002.txt, etc.
      -r, --rawtext         By default, a newline is appended to the text if it
                            doesn't already end with one. Use this flag to only
                            save the raw text.
      -t TIMEOUT, --timeout TIMEOUT
                            Number of seconds to wait for more Neo input before
                            terminating. The timer starts after the first input is
                            received. Default = 3 seconds.
      -w, --whisper         Only print warning and error messages. Stay silent
                            otherwise.

## Tested

Tested on the following:

OS X:
* OS X 10.11.3
* Python 2.7.11 (Homebrew)
* Python 3.5.1 (Homebrew)

Linux:
* Ubuntu 15.10
* TODO: Python 2 (Ubuntu)
* Python 3.4.3+ (apt-get)

NOTE: untested on other OSs.

## Licensed under GPL v3

Copyright 2016 by Amar P. Kurani.

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
