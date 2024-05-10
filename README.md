# Hand-Written-Recognition-using-IMU-sensor-
In this project we are developing a handwritten recognition system using Arduino BLE33 IMU sensors to capture motion data for numbers and alphabets, crucial for digitizing documents and gesture recognition.

# Harware used:
Arduino Nano 33 BLE

![download](https://github.com/Allenzzygeorge/Hand-Written-Recognition-using-IMU-sensor-/assets/148372527/81b7169d-5a29-44e3-8c81-f9d8d258ac8e)

# Software Used:
Arduino IDE for arduino communication

Google Colab or Jupyter notebook for Model training

![our_model](https://github.com/Allenzzygeorge/Hand-Written-Recognition-using-IMU-sensor-/assets/148372527/42cea844-ba06-4b42-a42a-e0f17bf18196)


# Procedures to Follow

1. Collect the IMU sensor data for training, here we have trainned for "a-z" and "0-9", you either use the dataset in the datasets folder or create your own dataset and convert it into jsoin fileusing the website (https://tinyml.seas.upenn.edu/magic_wand_capture.html)

2. Validate the IMU sensor data, if individual datasets are taken verify each json files and combine the entire files into a single json file

3. If you are using the dataset that we created navigate to datasets folder in that 'individual_letters' contains the datasets for individual letters and 'full_data' contains the combined valid datasets use the 'complete_data_combined.json' for training the model if you are not creating your own custom dataset.

4. To train the model check for codes in the 'python_codes' folder, to use a local server to train the model use jupyter notebook code with name 'Model_JN.ipynb', to train the model in cloud like google colab use the 'Model_GC.ipynb' for train the model and generate a tensorflow lite model for Microcontrollers.

5. Take the output 'magic_wand_model_data.cpp' and from the training part paste it in the arduino IDE part.

6. Run the 'arduino_code/Hand_written_imu'with the replaced 'magic_wand_model_data.cpp' part and do real time testing of you model. 

# Authors
Allen C George (allenc@iisc.ac.in)
Ranwin kumar (ranwinkumar@iisc.ac.in)
