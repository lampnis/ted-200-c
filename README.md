## Getting the temperature measurement from Thorlabs TED 200 C Temperature controller

Below there is just a code that calculates the $\beta$ value and temperature in Celsius depending on the resistance reading $R$ on instrument.

$\beta=\frac{\ln (R/R_0)}{\frac{1}{T}-\frac{1}{T_0}}$

$T(R)=\frac{\beta T_0}{T_0 \ln(R/R_0)+\beta}$

There is also a quick helper function to convert from Kelvin to Celsius and vice versa.

In the last `print` statement, change just the value of the first argument in function `get_temp()`, where you enter the actual reading that you get.

You can change the calibration (`B_val_g`) depending on the actual thermistor by supplying actual values from your specs.

I attach additional manuals, where you can read more about the actual setup that I was using.
