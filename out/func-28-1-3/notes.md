# func-28-1-3 Notes

2018-01-29 15:11:06

Run with arguments test/critiquepracticalreason_00_kant_64kb.c2cb-3200 --load-weights=out/func-28-1-2/weights-15000.h5

## Description

Added in two new LSTMs and reloaded weights from last run.

Disabled training on the 3 initial LSTMs and on encoder and decoder

Going well!

Restarted at 3000, having reenabled trainable flag for 
the initial LSTMs, allowing all LSTMs to refine themselves.

Restarted at 5450. Added 2 more LSTMs on the end, disabling the training 
of existing early and mid LSTMs.


Restarted at 9290 with a final wide LSTM on the end after disabling the training of all others

Didn't work due to a shape mismatch. Trying two new lstms instead of one large

Restarted at 12940 setting all LSTMs to trainable

At 18130 added two more LSTMs, disabling all others from training.


At 20290 enabled training on all the LSTMs. 

Finished running at 27830. The results are interesting. 
Unfortunately the time it takes to load the network to 
generate is very large. 