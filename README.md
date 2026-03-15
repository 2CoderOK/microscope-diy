# DIY Electronic Microscope (CCD Module + S-Video convertor)

<img alt="DIY Electronic Microscope" width="500px" src="https://github.com/2CoderOK/microscope-diy/blob/main/microscope_image.jpg" />

In the video below, I’ll show you how I built an optical-digital-analog microscope using an old photo enlarger, a camera lens, a CCTV camera, and an S-Video to VGA converter. 

I built this project specifically for soldering. Many budget digital microscopes suffer from latency and motion blur, which makes precision work incredibly difficult. By leveraging an analog CCTV camera and a direct VGA converter, this setup provides a lag-free, high-quality image for a fraction of the cost of high-end microscopes (around $20 for the purchased modules).

I’ll walk you through the process, including some soldering and 3D printing custom parts. All files required for 3D printing are placed inside the `stl` directory.

## 🛠 Hardware Components
* **CCD Module:** SONY 4140+811 HD 700TVL (Requires 12V)
* **S-Video to VGA Convertor:** ATIS VGA-AV (Requires 5V)
* **Lens:** Industar 61 2.8/50 (repurposed from an old Zenit camera)
* **Photo Enlarger:** Leningrad 2

## 🖨️ 3D Printed Parts
The custom parts were modeled in Tinkercad and printed on a Creality Ender 3. 
* **Lens Adapter:** An M42 to M39 thread adapter to mount the Industar lens to the photo enlarger.
* **CCD & OSD Housing:** A custom mount to securely hold the CCD module and enclose the OSD (On-Screen Display) keypad.
* **Top Cover:** A replacement lid for the enlarger head that holds the S-Video to VGA converter and the custom power distribution board.

## ⚡ Electronics & Soldering
* **OSD Keypad:** The camera module settings are controlled via a custom keypad. I soldered tactile buttons onto a single-sided PCB and wired it to the module using a repurposed Ethernet cable and heat shrink tubing.
* **Power Distribution (5V Step-Down):** Because the CCD module runs on 12V and the VGA converter requires 5V, I built a custom power board so both can run from a single 12V power adapter. It uses an LM7805 voltage regulator, a couple of capacitors, and DC in/out connectors.

## ⚙️ Calibration & Usage
* **Height & Macro Adjustments:** The main height and zoom are easily adjusted using the Leningrad 2's native vertical sliding mechanism.
* **Fine Focus:** Focus is dialed in manually using the focus ring on the Industar lens.
* **Image Tuning:** Using the custom OSD keypad, I recommend taking the camera out of "Auto" mode. Switching to daytime mode and manually tweaking the brightness and contrast yields a much better image for inspecting PCBs.

Here you can watch the video: [https://youtube.com/@coderok](https://youtu.be/W8HXRcmqQwQ)

[<img alt="DIY Electronic Microscope" src="https://github.com/2CoderOK/microscope-diy/blob/main/microscope_preview.jpg" />](https://youtu.be/W8HXRcmqQwQ)

OSD pinout:

<img alt="DIY Electronic Microscope" src="https://github.com/2CoderOK/microscope-diy/blob/main/osd_pinout.jpg" />

[<img alt="Buy me a coffee" height="50px" src="https://github.com/2CoderOK/jp-trainer/blob/main/yellow-button.png" />](https://www.buymeacoffee.com/coderok)
