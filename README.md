# Custom A1 Mini Camera Systen

This is my custom camera system design for the Bambu lab A1 Mini where I will use custom G-code to program the nozzle to tap into a camera switch after each layer of print. 
I will use a Raspberry Pi Pico to detect the switch through a GPIO pin and send a keyboard shortcut to my computer as a HID device. My computer will then take a frame from the camera, by either taking a screenshot of the webcam interface or by using custom software to control the camera and take a photo.
After each photo is taken, the printer will continue printing and at the end I will have lots of photos I can edit together to make a smooth timelapse of my prints.



# How it will work:

- Nozzle moves to specific positon between layers through my custom G-code and taps into the camera clicker
- Raspberry Pi Pico wired to the clicker detects the signal and sends command to computer
- Computer picks up the keybind and takes action (screenshot or take photo)
- Nozzle goes back to printing and repeats the process
- I will edit the photos together to make the timelapse

**I will need to design in CAD custom mounds for the switch and for the camera**


# Component BOM:

| Name | Use | Link | Price | US |
|------|-----|------|-------|----|
| Logitech C270 | Take photos of my prints | [link]() | £ | $ |
| Camera clicker | Register clicks from printer | [link]() | £ | $ |
| Raspberry Pi Pico | Act as a HID to send signal to computer | [link]() | £ | $ |
| 3D printed mounts | Secure clicker & camera | [link]() | £ | $ |

Total = £ or $


# Firmware

I will need to program the Raspberry Pi Pico to recieve the signal from the clicker and to act as a HID keyboard to send keystrokes to my computer via USB cable. I will likely program this in CircuitPython as I am relatively familiar with it.







## Rework criteria:

- Full image of your project/'s CAD
- Short description of your project and why you made it
- BOM in table format
- Wiring diagram for your full project

