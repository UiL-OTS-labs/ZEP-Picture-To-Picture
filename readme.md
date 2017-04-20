# ZEP; Picture to Picture
## Description:

Purpose of this ZEP experiment is to measure a participant's ability
to link one picture to another. For each trial three images are presented simultaneously.

Participant's task is to select which of the two images best match the
third image. Experiment is self-paced, has visual
appealing features, and some instruction.

## Installing and starting
* Download and install zep (1.14) [here](http://beexy.org/zep/wiki) for either Windows OS or a Debian based Linux OS
* Download and unpack this repository
* Run either `windows-terminal.bat` or `linux-terminal.sh` to start up a _command-line interface_ within the unpacked repository
* You can then start up the experiment by typing: `zep pictopic.zp` or `zep-1.14 pictopic.zp`

## Adding stimuli
Please add your own stimuli by populating the `stimuli/images` directory with your own images (svg or png) and update `stimuli/test_items.csv` and `stimuli/prac_items.csv`.

You might want to change `SCALING_FACTOR_FOR_IMAGES` in `modules/globaldefs.zm` if your largest image is bigger than 1/2 of the screen height.

## Changing settings
In `test/defs.zm` you can change switches for feedback, switches for prompts, and prompts. In this file you can also set small timing tweaks inter-stimulus interval.

## Control
Either use:
*   BeexyBox response buttons
*   Left and right shift
*   Use mouse to select picture

## Output: chosen value, correctness, and reaction time.

Author:
Chris van Run (UiL-OTS) <labman.gw@uu.nl>

Client:
-

Supervisors:
-
## Randomisation
Test trials are completely random (no pseudo-randomisation).

## Acknowledgements
* Efi Giannopoulou​ prompting the creation of this Boilerplate experiment.

## About Zep
Zep is a system for implementing and running (psycholinguistic) experiments. Zep delivers auditory, visual and cross modal stimuli, and provides interfacing with external hardware such as eye-trackers and button boxes. It is based on a multipurpose programming language (also called Zep) which enables you to implement not only experiments but other applications as well.

DISCLAIMER

This experiment script is released under the terms of the GNU General Public
License (see http://www.gnu.org/licenses/gpl-2.0.html). It is distributed in
the hope that it will be useful, but with absolutely no warranty. It is your
responsibility to carefully study and test the script before using it with
real participants.
