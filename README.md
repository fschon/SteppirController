# Steppir Antenna Controller - Remote low cost Steppir antenna controller. 

I recently acquired a 12 year old Steppir 3 element antenna missing the controller. Due to the age of the antenna, I did not want to invest in a new controller and so looked into the idea of using 3d printer electronics to build my own. 

This project uses a Big Tree Tech Octopus 1.1, a Raspberry Pi and Klipper, Moonraker and Node Red software as a replacement. Total cost so far is under $150. 

Using existing 3d solutions allows for off-the-shelf cheap hardware and software to control the stepper motors inside the EHUs. All current, speed, acceleration and positioning of the stepper motors is possible and gcodes can be used to position the element copper tape in the antenna tubes. The Octopus TMC2209 stepper drivers are also configured to use StallGuard which detects when the tape is fully retracted when calibrating and stops the motors from unnecessary straining, thus reducing load on the motor drive shafts which are know to fail on older Steppirs.

The controller can probably also be used to control a antenna rotator as well. By using either stepper motor controls, or the filament or bed heater outputs on the Octopus to control the rotor motor. This could potentially save additional hundreds of dollars on a rotator controller.

Because the controller uses a Node Red dashboard, the controller can be remotely operated and the controller electronics located closer to the antenna, alleviating the need to run long control cables to my shack.
