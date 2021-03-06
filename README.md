# Donkey 2

This is the default method to use the Donkey Car. 

* [Video tutorial.](https://www.youtube.com/watch?v=NGTbzfx7aL4&feature=youtu.be)
* [Video showing how to create a new car with different parts](https://www.youtube.com/watch?v=xqASPxPpkw0&t=91s)


# Get driving.

Run these commands to setup your donkey car app on your car's raspberry pi.

1. Create and activate your virtual environment.
   ```bash
   virtualenv env --python=python3
   source env/bin/activate
   ```

2. Dowload and install the dependencies for this car template.
   ```bash
   git clone https://github.com/autorope/donkey2.git
   cd donkey2
   pip install -r drive_requirements.txt
   ```
   
3. Run the drive script.
   ```bash 
   python drive.py
   ```


# Train an autopilot.

Here are the steps to train an autopilot on your computer after you've transfered the
the tubs from your car's pi to your laptop. 


1. Create and activate your virtual environment.
   ```bash
   virtualenv env --python=python3
   source env/bin/activate
   ```

2. Dowload and install the dependencies for this car template.
   ```bash
   git clone https://github.com/autorope/donkey2.git
   cd donkey2
   pip install -r train_requirements.txt
   ```

3. Train an autopilot
   ```bash
    python train.py /path/to/folder/with/tubs/*
    ```
