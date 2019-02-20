# MATRIX-Lite-Py
**Under Development**

# Roadmap
This roadmap is for achieving a basic implementation of the checklist below. **As this package develops, the API will improve and may change.**
- [ ] Leds
- [ ] Sensors
  - [ ] IMU
  - [ ] Humidity
  - [ ] Pressure
  - [ ] UV
- [ ] GPIO
- [ ] Microphones
  - [ ] Hal Mics
  - [ ] Alsa Mics

# Development Dependencies
Ensure you have a Raspberry Pi, attached with a MATRIX device, that's flashed with [Raspbian Stretch](https://www.raspberrypi.org/blog/raspbian-stretch/).

Install SWIG 
```bash
sudo apt-get install swig
```
Install pip3
```
sudo apt-get install python3-pip
```

## 1. Install MATRIX HAL
https://matrix-io.github.io/matrix-documentation/matrix-hal/getting-started/installation-package/

## 2. Clone & Build the repository
This will compile SWIG wrapper for HAL.
```
git clone --recurse-submodules https://github.com/matrix-io/matrix-lite-py
cd matrix-lite-py
make
```
<!-- 
longer git clone alternative:
git clone https://github.com/matrix-io/matrix-lite-py
git submodule init
git submodule update 
-->

## 3. Run the python script
```
python3 swigExamples.py
```

