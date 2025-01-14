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
- **OV5647 image-sensor, taken from a PiCamera-module **
- **LiPO Battery (1200mAh)**: For portability
- **Powerboost 1000c (Adafruit)**: Charges the battery with micro-USB.
- **Switch**
- **3D-printed casing (PLA)**: Holds all components, designed to perfectly snap into place inside the camera.

### **3D-Printed Design**
The casing is designed so that the sensor placement can be ajdusted for optimal focus, around the intended focal plane for the film. CAD files and dimensions are available in the `hardware/` directory.

---

## **Software**
1. The script requires the PiCamera-library and openCV which can be installed.
2. A Samba server-client solution is implemented to make file-sharing between the camera and a Windows system easy.

---

## **Implementation**

### **Hardware Assembly**
This setup requires some soldering but the system could of course run with a usb connected powerbank, if one small enough is accessible.

### **Software Configuration**
The software implementaion is straight forward. The system should run on 
1. Enable the legacy camera interface in the Raspberry Pi setup.
2. Configure Samba for seamless file sharing.
3. Run the Python script to test video capture functionality.

---

## **Results**
The camera produces digital photos with a vintage look that can only be achieved with the lens of an film camera. The photos automatically saves on my computer whenever the camera is in WiFi range.

---

## **Future Improvements**
- Add a **DC-DC buck converter** for optimal voltage regulation, enhancing system lifespan.
- Create a server for automated file organization across network devices.

---
