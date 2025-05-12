# Skyscan-tracker-
High speed multi spectral camera 
# SkyScan Tracker  
**An open-source, high-speed multispectral tracker for atmospheric phenomena (meteors, sprites, lightning).**  

![Device Render](images/skyscan_render.jpg) *[Exterior only, no PCB close-ups]*  

## **Key Features**  
- **Tri-band sensor array** (UV-Vis-NIR via Ximea xiSpec)  
- **AI-powered tracking** (Jetson Nano for anomalous motion detection)  
- **"Environmental RF Calibration"** (Helmholtz coils + SDR)  
- **Modular optics** (interchangeable lenses for wide/zoom FOV)  

---

## **Sanitized Block Diagram**  
```plaintext  
[UV-Vis-NIR Sensor] → [Jetson Nano] → [SD Card]  
       ↑                    ↑  
[LCTF/Filter Wheel]    [Helmholtz Coils]  
       ↑                    ↑  
[GPS/IMU]             [HackRF One (SDR)]  
