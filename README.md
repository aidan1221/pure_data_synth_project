old# pure_data_synth_project
final project for CS 510: Computers, Sound &amp; Music

### synth2.pd
- primary synth patch
    - Drum machine with two beats to select from
        - low/band/hi-pass filter control
    - Three oscillators, each with possible sine/square/saw waveform
        - low/band/hi-pass filter control
    - Random melody generator with key selection, +/- 2 octave selector
    - Frequency modulation control
    - Phaser effect by Pat
    - Internal and external audio recording and looping using recorder_looper patch by Trina

## Final Assessment
For this project we wanted to experiment with modular synthesis using Pure Data. At the end of the project, Aidan built the main patch for the synth body, including 3 oscillators to select between sine, square, and saw waves, a drum machine beat generator, hi/lo/band pass filter control for oscillators and drum bus, frequenecy modulation controls, and a random melody generator with major/minor key selection. Trina built a recorded audio looping playback patch so that internal audio could be recorded and looped. This can also record external audio from microphone input.
Aidan would have liked to implement envelope controls for amp level and filter cutoffs, as well as a more detailed melody generation system, possibly something along the lines of a chord selector and arpeggiator.
Trina would have liked to fine tune the timing on the looping/playback from recorded audio so that the loops were smoother and recording would stop automatically when the table size was reached. Additionally, possibly a larger instrument bank of recorded samples/one-shots to be able to add to recorded sections.
Pat put together two different sub-patch effects: a phaser and a delay/reverb effect with a lo-pass filter. He also, with Aidan’s help, was able to convert the audio digital converter signal of his guitar to the proper midi value needed so it could run through as input like everything else in the synth. The phaser was constructed using nine all-pass filters, an LFO wave, and coefficients to adjust the mix of the wet signal with the original signal, depth, rate, and shift. Pat wanted to use nine-all pass filters due to its unique sound, as most phasers use eight or sixteen filters to get four or eight poles, respectively. Luckily, pure data has a reverse pole object and real one pole object, which somewhat eliminated the math and more so only required understanding how a phaser works. The reverb effect was essentially made by using a delay line and experimentation of mixing feedback and previous signals with the current input signal. Putting a slight emphasis on a lo-pass filter helped eliminate some unwanted noise that took away from the “dreamy” and light sound that reverb touches on.

Pat wishes he would’ve had more time to create the phaser using an FFT and more math. It was great to achieve the sound that he ended up getting nonetheless. In addition, he also wishes he could’ve used his guitar in other ways too, such as taking its input values not solely for conversion, but as a way to act as a parameter that affected other elements of the synth, such as the rate of an oscillator or what kind of filter to use based on either the frequency or the velocity.
