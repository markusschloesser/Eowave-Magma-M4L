# Eowave Magma M4L/MaxforLive device
This is a maxforlive device to control the Eowave Magma from Ableton. The Magma is a 101-ish synth but has additional features that the original does not have, like 3 Envelopes (Amp, Filter and AD Pitch), 2 LFOs (syncable to Midi clock), Presets (!), additional Waveforms for the LFOs and is fully controllable over CC.
There are unfortunately a couple of peculiar issues when controlling it. See ISSUES here on Github.
I based my device on the fantastic M4L device by Dominik Bohn (https://nukemodular.gumroad.com) which is for the Roland SH-01a, and 
1. removed stuff the Magma does not have (Polyphony, Chords, Unison etc)
2. Added all the features from above that the Magma has (ENVs, LFOS etc)
3. changed all the CCs and added the ones for 2. 
4. Gave all parameters the proper order so that you can control it nicely from controllers
5. Named the parameter values where applicable (LFO waveforms, Octave tune and sub OSC tune) 

I tried contacting Eowave a couple of times to clarify strange behavior, unfortunately they never replied. So if you have any insights (especially any available Sysex calls for patch parsing), please, let me know! :-)

Unfortunately the manual, while very entertaining to read has lots of errors in it. ALL CCs are wrong (I checked the english, french and german version) and using trial and error I figured out the real CCs. THEN I found this in a french forum "
For those interested it works but you have to add 64 to the figure indicated.
For example for the Cutoff it will be number 65.
On the other hand VEL_VCA does not react unlike VEL_VCF but hey it is already good."
Here in the WIKI are the real CCs https://github.com/markusschloesser/Eowave-Magma-M4L/wiki/the-REAL-CC-values

Also to disable starting the internal sequencer to the midi clock, while still syncing the LFOs:"turn it on while holding down the [START] key, so that the sequencer becomes inactive, until the next "reboot" of the machine"

This is the actual Hardware device: http://www.eowave.com/synthesizers/magma/ 

