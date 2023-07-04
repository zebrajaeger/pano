# Pano

This repository represents an overview of the different subprojects related to my panorama workflow.

1) Take pictures: 
    1) Auto panoramic head: [ph3](https://github.com/zebrajaeger/ph3)
        - Shoot photos automatically
        - Java, Spring Boot, Angular, Arduino, C++
    1) Move panoramic head with a Joystick: [pi-pico-usb-joystick](https://github.com/zebrajaeger/pi-pico-usb-joystick)    
        - Precise Movement with [FrSky spare part](https://www.google.com/search?q=FrSky+Gimbal+M9+Hall+Sensor+Taranis+X9D+Plus).
        - USB HID Device, works on every platform
        - [CircuitPython for Raspberry Pi Pico](https://circuitpython.org/board/raspberry_pi_pico/)
    1) Develop: Remote connection to a i2c-bus: [remote-i2c](https://github.com/zebrajaeger/remote-i2c)
        - For Raspberry PI
        - Local machine high-level development with connection to a real device
    1) Optional: [GPS Position Sensor](https://github.com/zebrajaeger/i2c-gps)
        - Connect a GP-02 Module via I2C
1) Stitch photos to one big image
    - Kolor Autopano Giga (commercial, discontinued by GoPro)
    - <https://download.kolor.com/apg/stable/history>
1) Generate tilemaps and Viewer: [jsphere2cube](https://github.com/zebrajaeger/jsphere2cube)
    - Java
    - Uses [marzipano](https://www.marzipano.net/) and [pannellum]()
1) Viewer: [Modified Pannellum viewer](https://github.com/zebrajaeger/pannellum-modified)
    - It doesn't stop auto-orientation on zoom/move
1) Server to present the panos: [pano-server](https://github.com/zebrajaeger/pano-server)
    - Overview
    - Preview for shared panos via FB/Whatsapp etc.
    - NodeJs, Docker
1) Backup/Storage
    1) Fix picture links in .pano files from Autopano Giga with [Autoopano Path Relativizer](https://github.com/zebrajaeger/autopano-path-relativizer)
       - Java
       - CLI or "GUI"
