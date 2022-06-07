# Input-Prioritization-for-DL-systems
This work compares test input prioritization techniques of different types in terms of effectiveness and efficiency. In particular, we consider surprise adequacy, autoencoder-based, and similarity-based input prioritization approaches in the example of testing a DL image classification algorithm applied on MNIST, Fashion-MNIST, CIFAR-10, and STL-10 datasets. We use a modified APFD (Average Percentage of Fault Detected) as the test input prioritization performance measure to operationalize the effectiveness. 
We have used the Tensorflow framework as the backend to execute; kindly download the requiremnt.txt file to see all the package dependencies. We used NumPy, seaborn, and matplotlib python libraries. We imported Keras from TensorFlow for a deep learning library. 

We are adding instructions sequentially to run this project. Follow the instruction below. 

1) Download all the files, including zip files.
2) Unpack these files.
3) Install the packages according to requirement.txt.
4) The zip file of each three techniques consists of their respective python source code. It is better to make their store in separate. 
5) Run training_cnn.py to train CNN. Change the number of epochs if needed.
6) Run training_ae.py to train AE. Change the number of epochs if needed.
7) Run training_vae.py to train VAE. Change the number of epochs if needed.
8) Run calculate_sa.ipynb to calculate SA prioritizations using the trained CNN as well as predictions made by the CNN. Change the path to the trained CNN if needed. The results are saved in the temp folder.
9) Run calculate_sim.ipynb to calculate similarity-based prioritizations and choose the best one. The results are saved in the temp folder.
10) Run calculate_ae.ipynb to calculate AE-based prioritization. Change the path to the trained AE if needed. The results are saved in the temp folder.
11) Run calculate_vae.ipynb to calculate VAE-based prioritization. Change the path to the trained VAE if needed. The results are saved in the temp folder.
12) Run calculate_fig.ipynb to calculate the final figure using the results from the temp folder.
