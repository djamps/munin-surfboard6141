# Munin plugin for Surfboard 6141

This is a Munin plugin which monitors the following data on a Motorola Surfboard 6141:

1. Upstream/Downstream power
2. Upstream/Downstream bonding status
3. Downstream SNR
4. Downstream Codewords/sec (good, fixed, and bad)

# Requirements / Configuration

Requires Perl and the following perl modules:

1. LWP::Simple
2. Regexp::Common

No special config is needed, this is a drop-in plugin.

Please report any suggestions / bugs.

# Example output

```
uspwr4.value 43
uspwr1.value 43
uspwr2.value 43
uspwr3.value 43
multigraph surfboard6141_downstream_power
dspwr61.value 11
dspwr62.value 10
dspwr63.value 10
dspwr64.value 10
dspwr69.value 9
dspwr70.value 9
dspwr71.value 9
dspwr72.value 9
multigraph surfboard6141_downstream_snr
dssnr61.value 38
dssnr62.value 38
dssnr63.value 38
dssnr64.value 38
dssnr69.value 38
dssnr70.value 38
dssnr71.value 39
dssnr72.value 38
multigraph surfboard6141_downstream_codewords
dscodewordsgood61.value 8406938798
dscodewordsfixed61.value 51
dscodewordsbad61.value 579
dscodewordsgood62.value 8406105262
dscodewordsfixed62.value 148
dscodewordsbad62.value 1458
dscodewordsgood63.value 8406113332
dscodewordsfixed63.value 84
dscodewordsbad63.value 1630
dscodewordsgood64.value 8406122022
dscodewordsfixed64.value 120
dscodewordsbad64.value 1530
dscodewordsgood69.value 8406099938
dscodewordsfixed69.value 133
dscodewordsbad69.value 1559
dscodewordsgood70.value 8406101041
dscodewordsfixed70.value 62
dscodewordsbad70.value 1646
dscodewordsgood71.value 8406103291
dscodewordsfixed71.value 207
dscodewordsbad71.value 1639
dscodewordsgood72.value 8406130037
dscodewordsfixed72.value 374
dscodewordsbad72.value 3493
multigraph surfboard6141_bonding
dsnum.value 8
usnum.value 4
```
