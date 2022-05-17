# Eowave Magma M4L/MaxforLive device
<img width="1383" alt="Eowave Magma m4l Screenshot 2022-05-09 195159" src="https://user-images.githubusercontent.com/59286549/168923507-bfe66d03-a07e-4e13-bdb1-5997deea6d39.png">
This is a maxforlive device to control the Eowave Magma from Ableton. The Magma is a 101-ish synth but has additional features that the original does not have, like 3 Envelopes (Amp, Filter and AD Pitch), 2 LFOs (syncable to Midi clock), Presets (!), additional Waveforms for the LFOs and is fully controllable over CC.
There are unfortunately a couple of peculiar issues when controlling it. See ISSUES here on Github.
I based my device on the fantastic M4L device by Dominik Bohn (https://nukemodular.gumroad.com) which is for the Roland SH-01a, and 
1. removed stuff the Magma does not have (Polyphony, Chords, Unison etc)
2. Added all the features from above that the Magma has (ENVs, LFOS etc)
3. changed all the CCs and added the ones for 2. 
4. Gave all parameters the proper order so that you can control it nicely from controllers
5. Named the parameter values where applicable (LFO waveforms, Octave tune and sub OSC tune) 

Unfortunately the manual, while very entertaining to read has a couple of errors in it. ALL CCs are wrong (I checked the english, french and german version) and using trial and error I figured out the real CCs. THEN I found this in a french forum "
For those interested it works but you have to add 64 to the figure indicated.
For example for the Cutoff it will be number 65.
On the other hand VEL_VCA does not react unlike VEL_VCF but hey it is already good."
Here in the WIKI are the real CCs https://github.com/markusschloesser/Eowave-Magma-M4L/wiki/the-REAL-CC-values

Also to disable starting the internal sequencer to the midi clock, while still syncing the LFOs:"turn it on while holding down the [START] key, so that the sequencer becomes inactive, until the next "reboot" of the machine"

UPDATE: I met Marc from Eowave at this year's Superbooth, very lovely guy! He was kind enough to send me his MAX patch which he used to build all presets for the Magma back in the day. It supports all kinds of sysex for preset management etc 🤯😊😊. I will try to understand what he did and incorporate that into my device. If any experienced max dev would be willing to help, I'd be grateful!

This is the actual Hardware device: http://www.eowave.com/synthesizers/magma/ 

