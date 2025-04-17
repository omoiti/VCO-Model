# Verilog-A Behavioral VCO Model


## Specifications
This Verilog-A module implements a behavioral Voltage-Controlled Oscillator (VCO) with configurable frequency, jitter, and phase noise. 

| Parameter | Description | Units | Default Value |
| --------- | ----------- | ----- | ------------- |
|     `fc`    | Center frequency (operating frequency at 0V input)| Hz | 2G (2 GHz) |
|    `gain`   |		Voltage-to-frequency conversion gain|	Hz/V|	200M (200 MHz/V)|
|   `jitter`	|	RMS cycle-to-cycle jitter| Seconds	| 10 ps|
|   `seed`	|	Number seed for jitter | -|	100|
|  `vout_amp` |	Output voltage amplitude|	Volts|	1|
|  `trise` |	Output rise time|	Seconds|	1 ps|
|  `tfall` |	Output fall time|	Seconds|	1 ps|
|    `ttol`   |	Time tolerance for cross events (controls phase accuracy)|	Seconds | 0.5n (0.5 ns)|
|    `vtol`   |	Voltage tolerance for cross events|	Volts	|1f (1e-15 V)|
| `min_pts_update` |	Minimum points per period (controls simulation time-step)|	-|	64|
| `phase_noise_level` |		Phase noise power density at phase_noise_fm (white noise floor)|	1/Hz|	1e-10|
| `phase_noise_fm` |	Offset frequency for phase noise specification	Hz|	1M (1 MHz)|
|`flicker_noise_level`|Flicker noise coefficient for 1/f³ phase noise region|	1/Hz³ | 1e-15|


