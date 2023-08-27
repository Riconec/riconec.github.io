# Microswitches accuracy for Z endstop \ probe usage
## Contender list
- Omron D2F-01F Japan (China versions have different actuation force and considered subpar to Omron Japan)
- Omron D2HW-A201
- Omron D2HW-A231
- Kailh GM4.0 Red

## Test method used
Since Voron 0 is running klipper with slide-swipe probe mod it makes sense just to use `PROBE_ACCURACY` command. To have better result series of 100 used. `PROBE_SPEED` is set to 5mm\s because I found faster and slower speeds can impact the accuracy results. So ho,ing with fast initial tap and actual measurement at calibrated speed makes sense.

Resulting test command as follows: `PROBE_ACCURACY SAMPLES=100 PROBE_SPEED=5` 

### Omron D2F-01F
`// probe accuracy results: maximum 16.794375, minimum 16.775000, range 0.019375, average 16.788169, median 16.788750, standard deviation 0.003074`

### Omron D2HW-A201
![alt](microswitch_accuracy/D2HWA201D.jpg D2HW-A201)
`// probe accuracy results: maximum 16.788750, minimum 16.778125, range 0.010625, average 16.782444, median 16.781875, standard deviation 0.002536`
### Omron D2HW-A231
`// probe accuracy results: maximum 16.801250, minimum 16.788125, range 0.013125, average 16.792156, median 16.790937, standard deviation 0.003318`

### Kailh GM4.0 Red
`// probe accuracy results: maximum 13.122500, minimum 13.103125, range 0.019375, average 13.115475, median 13.115000, standard deviation 0.002359`
