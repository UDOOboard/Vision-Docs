
# OpenVINO&trade; toolkit

The UDOO Vision board is equipped with an Intel&reg; HD Graphics 500 GPU which is fully supported by the
[OpenVINO&trade; toolkit](https://docs.openvino.ai/latest/index.html), an open-source framework for optimizing and
deploy AI inference.

By looking at the [Get Started page](https://docs.openvino.ai/latest/get_started.html), you can retrieve all the
information you need to install and start playing with the Intel toolkit.


### Get started

Here are reported a non-exhaustive list of commands to perform a common installation of OpenVINO version 2021.4.689.\\
This installation has been succesfully performed on *Ubuntu 20.04*.

First of all, install latest update and then install the dependencies
``` bash
sudo apt update
sudo apt upgrade
sudo apt install software-properties-common apt-utils wget curl cpio lsb-release build-essential vim usbutils cmake rsync
                    openssh-client openssh-server libgtk-3-dev htop sudo python3.8 python3-virtualenv python3-pip
                    libssl-dev qt5-default qtbase5-dev git libusb-dev libmosquittopp-dev libgflags-dev
                    libqt5websockets5-dev zlib1g-dev
```

Then actually install the toolkit
```bash
curl https://apt.repos.intel.com/openvino/2021/GPG-PUB-KEY-INTEL-OPENVINO-2021 | sudo apt-key add -
sudo echo "deb https://apt.repos.intel.com/openvino/2021 all main" | tee /etc/apt/sources.list.d/intel-openvino-2021.list
sudo apt update 
sudo apt install intel-openvino-dev-ubuntu20-2021.4.689
```

Finally install external dependencies and setup the environment so that the the framework will be automatically loaded
when new terminal are opened for the current user
```bash
cd /opt/intel/openvino_2021/install_dependencies
sudo -E ./install_openvino_dependencies.sh -y
sudo -E ./install_NEO_OCL_driver.sh -y
bash -c 'echo -e "\n\n# Loading OpenVINO variables\nsource /opt/intel/openvino_2021/bin/setupvars.sh\n"' >> $HOME/.bashrc
```