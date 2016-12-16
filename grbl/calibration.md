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
