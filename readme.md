In our Submission we provide 4 python notebooks:
1. Task_1_1_Calc_emebddings_and_accuracy_both
2. Task_1_1_with_uploaded_embeddings
3. Task_1_2_Calc_emebddings_and_accuracy_both
4. Task_1_2_aacuracy_with_uploaded_embeddings


One pair of notebooks for each of the two tasks of Part 1.
One notebook has code to verify accuracy from the uploaded embeddings, and the other one has code to calculate embeddings and accuracy both. The former one requires lesser time and no GPU, while the later one requies GPU for faster execution but still requies approximately 40-50 minutes to run on the google colab with T4 GPU.

The drive link has the embeddings in it which can be downloaded and used to verify the accuracies, but the paths must be verified before running the code. We also provide the resent model, and the pickle file of the prototypes obtained after TASK 1.1, which should be downloaded and used in task 1.2.

Drive Link: https://drive.google.com/drive/folders/1PxlJzTb1fcF-D0O0j1EEs1J5SkjZo7sM?usp=sharing

To run the first notebook, "Task_1_1_Calc_embeddings_and_accuracy_both", you will need part_one_dataset and resnet.pth from the Drive. Update the file paths in the code if necessary. Using these files, the code will generate embeddings as .npy files, compress them into a .tar.gz archive, and save it. Finally, the embeddings will be used to calculate and display accuraciess, and the means will be saved as a mean_after_1.1.pkl file.

To run the second notebook, "Task_1_1_with_uploaded_embeddings", you will need part_one_dataset and Data1Embd from the Drive. Update the file paths in the code if necessary. The code will use the embeddings from the Data1Embd folder to calculate and display accuracies.

To run the third notebook, "Task_1_2_Calc_embeddings_and_accuracy_both", you will need part_two_dataset, Data1Embd, mean_after_1.1.pkl, and resnet.pth from the Drive. Update the file paths in the code if necessary. Using these files, the code will generate embeddings from the second dataset (D11–D20) as .npy files, compress them into a .tar.gz archive, and save it. Finally, using these embeddings, Data1Embd, and mean_after_1.1.pkl, accuracies will be calculated and displayed.

To run the fourth notebook, "Task_1_2_aacuracy_with_uploaded_embeddings", you will need part_two_dataset, Data1Embd, Data2Embd and mean_after_1.1.pkl from the Drive. Update the file paths in the code if necessary. The code will use the embeddings from the Data1Embd, Data2Embd folder to calculate and display accuracies.



The dependecies are:
torch
numpy
torchvision
PIL
tarfile
os
sklearn
pickle
cv2
matplotlib
