## ( QUADRUPLE ROBOT DOG - INSPIRED BY Unitree ): Open-sourced ##

As you may have read the repository title, this is my FIRST an open-sourced robot dog project. If I have lacked any resources, please message me in Reddit **( https://www.reddit.com/user/Severe_Package6618/ - Display name is MiniGriphy )**

<p align="center">
  <img src="RD_Image_References/Reddit_Profile_Picture.jpg" width="400">
  <br>
  <em>Reddit Account</em>
</p>

---

## ( Preface ):
In order for this project to work, I really recommend you using a 3D printer that has a dimension of 260 x 260 x 300 mm^3 (the one I'm using is Creality). If you don't have one, it's fine, just try to adjust the component on the printing platform **diagonally** until the part fits on the it perfectly without crossing the boundary. 

This project relies on 12 servos/motors, **DS3235 (a torque of 35kg/cm)**, you can purchase it from Amazon, AliExpress, or any websites that are completely safe. The reason why we need DS3235 is that we want a strong torque that would lift at least 1 kilogram (kg) of body weight. Even the servos can easily this weight, we also need to ensure that when adding electronics (e.g., batteries, cables, microcontroller, AI vision, etc), the DS3235 servos are still be able to lift them. 

And to extract the servos' full potential, we have to use 6.8 V - 7.4V (volts) 20A (or higher current) power supply or battery (note: this would add additional weight to the robot, and we need to be constantly cautious about the total weight while making this project). Otherwise, if you have, let's say, a 5V 15A power supply, the servos won't be able to exert all its torque power, meaning it would be slightly tedious to conduct the heavy-lifting. 

Additionally, I recommend a power setup that can endure 20 Amps of current so your controller board's traces do not burn out. A standard PCA9685 board safely accepts only up to 10 Amps; high-current servo spikes will quickly melt its traces. While adding a capacitor can smooth out voltage drops, a much simpler control solution is the Hiwonder LSC-32 32-Channel Controller. The LSC-32 handles power much better than a PCA9685 thanks to **integrated 6-channel over-current fuses**. To safely reach a full 20 Amps without tripping those built-in fuses, USE a **split-power** method: run the servo signal lines to the LSC-32, but wire the servo power leads directly to a 20A external terminal block. 

---

## ( What Do We NEED for The Quadruple Robot Dog; resources requirements? ):
- A 6.8V - 7.4V 20A power supply or battery.
- Hiwonder LSC-32 32-Channel Controller (Alternative: PCA9685 driver board can be acceptable if you have solutions to prevent current spike)
- 12 DS3235 Servos/Motors
- CAD parts/components (Robot Dog)
- A camera feed

---

# ( Before We Begin, I Just Want to Show You My Legacy Designs - Neglect this if you don't really care. ): 
