# Two-Stage-CMOS-OpAmp
Design and Simulation of 2-stage Operational Amplifier using LTspice. Achieved required gain, GBW, phase  argin and CMRR etc.
# Design description
This project used 180nm technology to build a well compensated OpAmp device features of the design are:
1. **Two stage amplification**:
     - Amplification is done in two stages. First is differential stage which amplified the differential input while in the second stage CS-amplifier has been used          to amplify the output of 1st stage.

2. **Miller compensation**:
     - The problem with two stage amplification is that at each gain stage sytem produces LHP poles that create phase lag in system and making system unstable.
     - To overcome this problem Miller capacitor(Cc) is used that increases the separation between the two poles and reduces the phase lag and increases stability.
     - Using miller capacitance increased the bandwidth of system so system can work fine for wider frequency range.
     - Miller compensation has increased the stability of system but it also creates a feedforward path and at high frequencies signal can sompletely bypass the             second stage. It creates an RHP zero that causes a phase lag and can effect the stability of system at high frequencies.
       
3. **Nulling resistor":
     - To nullify the effect of rhp zero a nulling resistor(Rz) is applied in series with Cc.
     - By choosing right value Rz the RHP zero is shifted to infinity and phase lag created by the zero is cancelled, hence phase margin increase.

# Circuit:
  <img width="1700" height="1050" alt="OP-Amp circuit" src="https://github.com/user-attachments/assets/32f8c573-a6e1-44df-90bf-df995846b702" />

# Applications
Miller-compensated two-stage op-amps are commonly used in Analog-to-Digital Converters (ADCs) & Digital-to-Analog Converters (DACs), Voltage regukation and Signal Conditioning & Buffering etc.

