# Rydberg Stark decelerator

## main.lvproj
## - create_wf.vi

Use the 'input' tab to specify the electrode configuration and desired acceleration/ deceleration stages.   The electrodes are equally spaced and grouped into cells of 'n' electrodes, where every i'th electrode is connected to the (i + n)'th. 

After making changes to the input settings ensure that the 'valid' indicator is lit then press 'Build' to solve the equations of motion for each stage (output to the 'sequence' tab) and to find the position of the trap centre as a function of time.

The trap position is translated into its phase with respect to the position of each electrode, which in turn gives the electrode waveforms (these are displayed on the 'electrodes' tab).  The waveforms can be linearly ramped on and off using the  'apply ramp' settings.

The 'correction' tab shows the waveform for the top electrode, which modulates to correct for a weakening of the trap as it passes over the regions between electrodes.  The frequency of the correction waveform is n times larger than that for the electrodes.  An arbitrary function that varies with either or both the trap position (x) and time (t) can be added to this. 

To view the changes, press 'Build' after modifying the input, ramp, add function, amplitudes, and offset settings. 

Waveforms scaled to between +/- 1.  Set amplitude and offset with hardware.

Save as a *.wf file (XML).

NB.  The functions of this vi are available for use as a subVI in wf_tools:create.vi
 


