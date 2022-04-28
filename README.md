# Input-Prioritization-for-DL-systems
This work compares test input prioritization techniques of different types in terms of their effectiveness and efficiency. In particular, we consider surprise adequacy, autoencoder- based, and similarity-based input prioritization approaches in the example of testing a DL image classification algorithm applied on MNIST, Fashion-MNIST, CIFAR-10, and STL-10 datasets. We use a modified APFD (Average Percentage of Fault Detected) as the test input prioritization performance measure to operationalize the effectiveness. 
We have used the Tensorflow framework as the backend to execute; kindly download the requiremnt.txt file to see all the package dependencies. We are adding sequncially instruction to run this project. Follow the instruction below. 

1) Run training_cnn.py to train CNN. Change the number of epochs if needed.
2) Run training_ae.py to train AE. Change the number of epochs if needed.
3) Run training_vae.py to train VAE. Change the number of epochs if needed.
4) Run calculate_sa.ipynb to calculate SA prioritizations using the trained CNN as well as predictions made by the CNN. Change the path to the trained CNN if needed. The results are saved into tmp folder.
5) Run calculate_sim.ipynb to calculate similarity-based prioritizations and choose the best one. The results are saved into tmp folder.
6) Run calculate_ae.ipynb to calculate AE-based prioritization. Change the path to the trained AE if needed. The results are saved into tmp folder.
7) Run calculate_vae.ipynb to calculate VAE-based prioritization. Change the path to the trained VAE if needed. The results are saved into tmp folder.
8) Run calculate_fig.ipynb to calculate the final figure using the results from tmp folder.
