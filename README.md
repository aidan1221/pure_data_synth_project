# pure_data_synth_project
final project for CS 510: Computers, Sound &amp; Music


 ### filter_abs.pd
 - abstraction for three way switch between high, band, and low pass filter

 ### osc_abs.pd
 - abstraction for three-way switch between sine, saw, and square wave


### synth1.pd
- main synth patch
    - on/off switch, volume slider for main amp control
    - two oscillators, each with three-way switch for square/sine/saw wave
    - hi pass, low pass, bandpass filter selector
    - notein object for midi keyboard use. Optional midi note slider and random midi note generator functions (not-currently attached to midi note send)


### snare_looper.pd
- abstraction to open and play a wave file in a loop


### recorder_looper.pd
- abstraction to record sounds and play in a loop. Multiples can be used at once.
    - start playing as soon as recording is finished option
    - start recording option
    - stop recording option--can't be pressed until after recording is started
    - play recording in a loop option
    - stop playback option
    - can stop and start multiple times

### synth2.pd
- second iteration of primary synth patch
    - now with drum machine with two beats to select from
        - added filter control for drum bus
    - added melody sequencer with pattern selector
    - main tempo control for melody sequencer and drum machine

## Final Assessment
For this project we wanted to experiment with modular synthesis using Pure Data. At the end of the project, Aidan built the main patch for the synth body, including 3 oscillators to select between sine, square, and saw waves, a drum machine beat generator, hi/lo/band pass filter control for oscillators and drum bus, frequenecy modulation controls, and a random melody generator with major/minor key selection. Trina built a recorded audio looping playback patch so that internal audio could be recorded and looped. This can also record external audio from microphone input.
Aidan would have liked to implement envelope controls for amp level and filter cutoffs, as well as a more detailed melody generation system, possibly something along the lines of a chord selector and arpeggiator.
Trina would have liked to fine tune the timing on the looping/playback from recorded audio so that the loops were smoother and recording would stop automatically when the table size was reached. Additionally, possibly a larger instrument bank of recorded samples/one-shots to be able to add to recorded sections. 
