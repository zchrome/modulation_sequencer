# Modulation Sequencer

Max for Live modulation sequencer Audio Effect device for Ableton Live.

<img width="514" height="189" alt="modseq_screenshot" src="https://github.com/user-attachments/assets/6e202502-7fe5-4657-8ae4-1823c3170f8c" />

Built with Max 8.6.4 and Ableton Live 12. No guarantees on other versions!

Download from the redist folder.

## Features

### Four modes for advancing the sequence:

**MIDI** advances on MIDI messages (note on, note off or both). User can set a count to advance after a certain number of note events, default is 1.  
**Seq** runs the sequencer on the Ableton clock, supports note value or free-running modes.  
**Gate** is similar to _Seq_ mode, but only advances when a MIDI note is held (analogous to an arpeggiator).  
**Manual** mode sets the step manuall with a knob (possible to automate or modulate).  

**Smoothing** and **jitter** controls to effect the modulation signal.  
Global **depth** control.  
**Sorting**, **randomization** and **scramble** functions to change all step values.  
Control of **step values** from multislider or fine-tune control with numboxes.  
Working **undo** buffer for the sequencer step values.  

**Known issues (August 2025)**:

- Manual mode does not respect / use the loop points
- Visual issue with sequencer starting from step one when loop starts at a higher sequence number and device is set to reset on transport
- Jitter applies modulation signal when sequencer is not running
- Warning in Max console relating to detection of track which device is residing on
- Untested behaviour when moving the loop points with the sequencer running
- Not audio rate!
