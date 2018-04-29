# buildLibrealsense2TX
Build librealsense 2.0 library on the NVIDIA Jetson TX2 Development kit.  Intel RealSense D415 cameras.

This is for version L4T 28.2 (JetPack 3.2)
librealsense v2.10.4

$ ./buildPatchedKernelTX.sh

<h2>Install librealsense 2.0</h2>
To install the librealsense library:

$ ./installLibrealsense.sh

<h2>Fix Error</h2>

1. Error: Failed to fetch http://ports.ubuntu.com/ubuntu-ports/dists/xenial/main/binary-amd64/Packages  404  Not Found [IP: 91.189.88.150 80]<h1>

$ sudo vi  /etc/apt/sources.list

Edit

deb url 

to 

deb [arch=arm64] url

For example, change

deb http://ports.ubuntu.com/ubuntu-ports/ xenial main restricted universe multiverse

to

deb [arch=arm64]  http://ports.ubuntu.com/ubuntu-ports/ xenial main restricted universe multiverse
