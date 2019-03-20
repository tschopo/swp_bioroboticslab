# Tracking bees in a tupe

Our aim is to track bees with Deep Learning Computer Vision Pipeline and grap ID and movement.
![Alt text](img/detected.png?raw=true "Beetracking")

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites
1. Software
First you need to have Python 3.7 (2.6 not tested, yet). (Anaconda is also a good solution)

Install diktya, Keras, OpenCV, dll first.

For this Jupyter Notebook you will need following dependencies:
Install with pip from github:

pip install --user git+https://github.com/BioroboticsLab/bb_utils.git      
pip install --user git+https://github.com/BioroboticsLab/bb_binary.git          
pip install --user git+https://github.com/BioroboticsLab/diktya.git     
pip install --user git+https://github.com/BioroboticsLab/bb_pipeline.git    
pip install --user git+https://github.com/BioroboticsLab/bb_tracking.git   
pip install --user git+https://github.com/BioroboticsLab/bb_behavior.git   
pip install --user git+https://github.com/BioroboticsLab/bb_trajectory.git     

You use an Apple and got a compiler problem with bb_binary?
Build capnp manually by:
curl -O https://capnproto.org/capnproto-c++-0.6.1.tar.gz
tar zxf capnproto-c++-0.6.1.tar.gz
cd capnproto-c++-0.6.1
./configure
make -j4
make install
pip install pycapnp

For Windows:
https://capnproto.org/install.html#installation-windows

2. Video path
We have set the path to /videos. You can easily change this path in jupyter file if needed.

3. BeesApp.apk
This app will help you to identify the bee for your test data sheet.
![Alt text](img/tagging.png?raw=true "Manually tag of a bee" height="50")

### Installing

Use git to download this repository (or download and unzip it).

Start Jupyter Notebook:
- open terminal
- start JN by typing

```
jupyter notebook
```

start Jupyter file. 
Done.

## Running the tests

If your video path is set correctly you can start each box by hitting Shift+Return from up to down.

### Break down into end to end tests

Take a coffee if you have a lot of clips. I may take a while to track all bees. We used around 200 clips and it took 1 hour to track all bees.

## Built With

* [Jupyter](https://jupyter.org) - Jupyter Notebook
* [Python](https://www.python.org) - Python

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

No versioning used.

## Authors

* **swp_bioroboticslab** - FU Berlin Computer Science

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Thanks to the FU Berlin bioroboticlabs group to provide us with their data and knowledge.

## FAQ
Do I need some more ressources? 
- Yes, we haven't included any video files. We worked with .h264 files to track bees.
- BeeApp.apk to track bees manually. 
Furthermore, coffee is never bad at all. 

What is included?
One main notebook file and the .dll file. (needed) 
CSV files with tracking, detection and test results. (not needed, bc you need to compute them with your clips)




