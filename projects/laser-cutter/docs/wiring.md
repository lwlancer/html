# Wiring and Signal Conditioning

## Power
- Source: printer 24 V rail.
- Buck: set to 12.00 V → LaserTree driver input rated 12 V 3 A.

## PWM Enable
- Board: Voxelab H2.
- Observed: ≈ 20 Hz PWM with unusual ±24 V swing vs board GND.
- Network: simple RC to invert/attenuate to TTL and filter HF noise.
- Current notes: divider roughly “10 k / 20 k”, C ≈ 10 nF. **To verify with scope.**
- Grounding: all returns to printer GND labeled supply pin.

## Safety
- External power interrupt with LED enable indicator.
- Interlocks and e-stop planned with controller upgrade.

## To Add
- Annotated schematic PDF.
- Scope screenshots for raw vs conditioned PWM.
- Final resistor and capacitor values with tolerances.
