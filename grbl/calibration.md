#Calibration

curr_steps_per_mm = steps/mm in current configuration
start_pos_grbl = starting position reported by software
end_pos_grbl = end position reported by software
start_pos_physical = actual/physical start position
end_pos_physical = actual/physical end position

steps/mm = (curr_steps_per_mm * (end_pos_grbl-start_pos_grbl)) / (end_pos_physical - start_pos_physical)



X and Y are set to 8x stepping - no jumpers
Z is set to 2x stepping - jumper
This configuration means that all three axes have a similar steps/mm, i.e. 40 steps/mm, 40 steps/mm and 49 steps/mm for X, Y and Z, respectively.


## Current Calibration

```
$0=10 (step pulse, usec)
$1=25 (step idle delay, msec)
$2=0 (step port invert mask:00000000)
$3=0 (dir port invert mask:00000000)
$4=0 (step enable invert, bool)
$5=0 (limit pins invert, bool)
$6=0 (probe pin invert, bool)
$10=3 (status report mask:00000011)
$11=0.010 (junction deviation, mm)
$12=0.002 (arc tolerance, mm)
$13=0 (report inches, bool)
$20=0 (soft limits, bool)
$21=1 (hard limits, bool)
$22=1 (homing cycle, bool)
$23=0 (homing dir invert mask:00000000)
$24=100.000 (homing feed, mm/min)
$25=1000.000 (homing seek, mm/min)
$26=250 (homing debounce, msec)
$27=5.000 (homing pull-off, mm)
$100=40.000 (x, step/mm)
$101=40.000 (y, step/mm)
$102=49.673 (z, step/mm)
$110=5000.000 (x max rate, mm/min)
$111=5000.000 (y max rate, mm/min)
$112=2500.000 (z max rate, mm/min)
$120=50.000 (x accel, mm/sec^2)
$121=50.000 (y accel, mm/sec^2)
$122=50.000 (z accel, mm/sec^2)
$130=200.000 (x max travel, mm)
$131=500.000 (y max travel, mm)
$132=200.000 (z max travel, mm)
```
