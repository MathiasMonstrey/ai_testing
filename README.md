# Hello Spot: Boston Dynamics API Tutorial

This is an example code to show how to interact with a Spot robot using the Boston Dynamics API.

The `hello_spot` function performs various tasks with the Spot robot, such as establishing connection, powering on/off the robot, making it stand, twist and change its height, capturing images from the robot, and saving the images to disk.

## Installation

Before running this code, please ensure you have Python 3.6 or later installed. You can install the necessary dependencies by running:

```sh
pip install bosdyn-client PIL
```

Please note that the `bosdyn-client` library is required to communicate with the Spot robot, and the `PIL` (Pillow) library is needed to handle images.

## Usage

You can run the program from the command line with:

```sh
python hello_spot.py -s --save-path /path/to/save/images
```

Here, the `-s` option tells the program to save images taken by Spot, and the `--save-path` option lets you specify the directory where images will be saved.

Please replace `/path/to/save/images` with the actual path on your system where you want the images to be saved.

## Functionality

The code demonstrates how to:

1. Establish connection with the Spot robot.
2. Authenticate the client and sync time with the robot.
3. Verify if the robot is estopped.
4. Acquire and manage the lease for controlling the robot.
5. Power on and off the robot.
6. Command the robot to stand in different positions.
7. Capture an image using the robot's camera and display it.
8. Save the captured image to a specified location.
9. Log a comment to the robot's log.

## License

This software is provided under the Boston Dynamics Software Development Kit License. The terms and conditions for use are specified in the file 20191101-BDSDK-SL. Please make sure to read them before using the software.

## Disclaimer

The authors are not responsible for any harm or damage caused by this software to the Spot robot or any other Boston Dynamics products or systems. Always ensure safety protocols are followed while operating the robot.
