# Digitalized-8mm-Camera
The revival of a vintage analog camera using a small single-board computer.
---

## **Introduction**
This project uses a Raspberry Pi Zero W and an OV5647 image sensor. The components fit inside a 3D-printed Super 8mm film casing. The modified camera records digital video files, preserving the vintage analog look of the Super8 camera.

### **Highlights**
- Replaces traditional Super 8mm film with a digital image sensor.
- 3D-printed casing holds all the components.
- Wireless connectivity allows easy file-sharing.

- ## **Hardware**

### **Component List**
- **Raspberry Pi Zero W**: A compact single-board computer that fits inside the camera.
- **PiCamera Module (OV5647 sensor)**
- **LiPO Battery (1200mAh)**: For portability
- **Powerboost 1000c (Adafruit)**: Charges the battery with micro-USB.
- **Switch**
- **3D-printed casing (PLA)**: Holds all components, designed to perfectly snap into place inside the camera.

### **3D-Printed Design**
The casing is designed so that the sensor placement can be ajdusted for optimal focus, around the intended focal plane for the film. CAD files and dimensions are available in the `hardware/` directory.

---

## **Software**

### **Setup**
1. Flash **Raspbian OS** onto the Raspberry Pi.
2. Establish a WiFi connection and enable SSH.
3. For windows systems **Samba** is used for file sharing. If using Linux SCP can be easily used for this purpose.
4. The provided Python script (`software/camera_script.py`) covers all basic features of the camera.

### **Python Script**
- The script configures the image sensor and captures video files.
- Outputs are saved in a shared directory accessible via the network.

---

## **Implementation**

### **Hardware Assembly**
1. Solder the LiPO battery to the power management module.
2. Connect the battery and module to the Raspberry Pi through a switch.
3. Use calculated dimensions to assemble the 3D-printed casing.
4. Position the image sensor at the correct focal length using focal plane calculations.

### **Software Configuration**
1. Enable the legacy camera interface in the Raspberry Pi setup.
2. Configure Samba for seamless file sharing.
3. Run the Python script to test video capture functionality.

---

## **Results**
- Fully functional digital recording system inside a vintage Super 8mm camera.
- High-quality video files stored and accessible via WiFi.

---

## **Future Improvements**
- Add a **DC-DC buck converter** for optimal voltage regulation, enhancing system lifespan.
- Create a server for automated file organization across network devices.

---

## **Gallery**
- Photos of the modified Super 8mm camera.
- Images of the 3D-printed casing and hardware assembly.
- Screenshots of video output quality.

---

## **License**
This project is open source under the [MIT License](LICENSE).

---

## **Contact**
For questions or collaboration opportunities, feel free to reach out or submit an issue on this repository.

---

## **Acknowledgments**
Special thanks to open-source communities and resources that made this project possible.

