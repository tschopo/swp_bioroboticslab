# swp_bioroboticslab

Installation der nötigen Softwarekomponenten
Dependencies:
diktya, Keras, OpenCV
https://github.com/BioroboticsLab/bb_utils.git
https://github.com/BioroboticsLab/bb_binary.git
https://github.com/BioroboticsLab/diktya.git
https://github.com/BioroboticsLab/bb_pipeline.git
https://github.com/BioroboticsLab/bb_tracking.git
https://github.com/BioroboticsLab/bb_behavior.git
https://github.com/BioroboticsLab/bb_trajectory.git

Probleme bei bb_binary für mac und windows: capnp muss manuell gebaut werden:
Für mac:
curl -O https://capnproto.org/capnproto-c++-0.6.1.tar.gz
tar zxf capnproto-c++-0.6.1.tar.gz
cd capnproto-c++-0.6.1
./configure
make -j4
make install
pip install pycapnp

Für windows:
https://capnproto.org/install.html#installation-windows
