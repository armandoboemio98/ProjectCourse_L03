
# Real-time Virtual Bass Enhancement

Virtual bass enhancement system for real-time applications

## Description
The real-time Virtual Bass Enhancement system allows to increase the perception of low frequency when using small loudspeakers, exploiting the missing fundamental theory.
It works in three modalities: NLD, Phase Vocoder, Hybrid.

The application has five tunable parameters (three knobs and two switch) that the user can tweak in real time:
* Crossover cut-off frequency
* Harmonics low-pass frequency
* Gain
* Harmonic generation mode
* Bypass

An in-depth explanation on how those parameters affect the sound is presented in the attached paper.


## Getting Started

### Dependencies

* MATLAB 2021 (older versions may present minor compatibility issues)
* MATLAB Audio Toolbox

### Executing program
#### If the user is familiar with the MATLAB Audio Toolbox:
* run 'tb.m' to initialize the Audio Testbench environment;
* Choose input and output devices and the audio track;
* Start the test, tweak parameters, close when done. 

#### If the user is not familiar with the MATLAB Audio Toolbox:
* run 'tb_play.m';
* Select the input audio track(wav, mp3, m4a, mp4) from the explorer;
* Tweak parameters. The script handles the audio device input and output selection, and also the buffer length choice.

## Help

The code performs significantly better with a buffer size equal to 1024. Changes to that size may affect the quality of the bass enhancement.
Check the [Documentation](https://github.com/armandoboemio98/ProjectCourse_L03/blob/main/documentation.md) for more information on the internal module structure. 

## Authors

Armando Boemio (armando.boemio@mail.polimi.it)

Gabriele Maucione (gabriele.maucione@mail.polimi.it)
