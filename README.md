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


### synth2.pd
- second iteration of primary synth patch
    - now with drum machine with two beats to select from
        - added filter control for drum bus
    - added melody sequencer with pattern selector
    - main tempo control for melody sequencer and drum machine
