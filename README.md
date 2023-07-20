# Smithchartaid
Smithchartaid is a utility that aids a design requiring a Smith Chart. It works on the Windows OS.
It was developed as a Windows Application in Visual Studio 2022 Ver 17.6.3 using the Target framework
.NET framework 4.8.04084.

The Smith Chart Aid UI overlays user specified impedance or admittance points and other useful graphics on a Smith Chart.
The underlying Smith Chart images (with black lines or colored lines) were generated in a separate program, saved, and
then included as a Resource within the application.

The Smith Chart Aid UI includes several panels. Up to four values of impedance or admittance (RX<n>, GB<n>) may be
entered (via their 'Enter' button) and each of these has a unique background color. Clicking on their respective
'Enter' button places their point on the chart, colored identically to their background color. Each RX<n>, GB<n>
UI panel includes a 'Parms' button. When clicked, scaled parameters for the impedance (or admittance) values are
provided in a pop-up window and include: 
  - Reflection Coefficient,
  - Standing Wave Ratio, and
  - Return Loss.

User Interface (UI) aids include:
  - 'Rotations Methods' UI to perform Operations on a point such as:
     1. rotating a point via the 'ROT Z,Y UI panel or
     2. aiding in double stub tuning provided by the UI panel whose headings include 'Mov B To Rot=1 Circle',
        'Select Root', and 'Rotate by -Rot Val'.
  - 'Medium Parameters' UI to calculate wavelength of the medium.
  - 'Unnorm <> Norm Conversion' UI to compute an unnormalized impedance (or admittance) given a transmission line
    characteristic impedance (or admittance) Z0,Y0, and a normalized impedance (or admittance) value specified in
	any of the RG<n>, XB<n> UIs, by selecting the n subscript value.  This UI also computes an inductive or
	capacitive value of the Unnormalized quantity given the frequency entered in the 'Medium Parameters' UI
  - 'Stub Length' UI that computes the length of a shorted-end or opened-end stub in units of wavelength.
  - 'Calculator' UI that computes:
     1. addition of two complex numbers
	 2. recprocal of a complex number
	 3. capacitive reactance and its resonant inductance given capacitance and frequency
	 4. inductive reactance and its resonant capacitance given inductance and frequency
	 5. converting fractional-wavelength to length
	 6. converting length to fractional-wavelength
	 7. converting fractional-wavelength to angle
	 8. converting angle to fractional-wavelength
	 9. normalized impedance given VSWR and an angle
  
At anytime, the Smith Chart may be reset by clicking on the 'Reset' button that clears all chart plots.
Values in the panel areas and their associated variables are not cleared.

There are help buttons identifed with a question mark '?' in all of the UI panels.
