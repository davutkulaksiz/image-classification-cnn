The contents of this file is moved to the README.md for better formatting. Look at the preview of README.md

# Image Classification with Convolutional Neural Networks

This project is an exploration of image classification using **Convolutional Neural Networks (CNNs)** using a deep learning framework called **PyTorch**. It implements and compares various CNN architectures with and without residual connections, different learning rates and batch sizes, and the use of dropout. The project also explores transfer learning with a pre-trained **ResNet-18** model.

## Requirements

This project requires:

- **Python 3**
- **PyTorch with CUDA**: Install it using `pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117`
- **matplotlib**: Install it using `pip install matplotlib`

## Dataset

The dataset, Micro_Organism, contains images of 8 categories of bacteria: Amoeba, Euglena, Hydra, Paramecium, Rod bacteria, Spherical bacteria, Spiral bacteria, and Yeast. The images should be arranged in the following directory structure:

<pre>
Micro_Organism/Amoeba
Micro_Organism/Euglena
Micro_Organism/Hydra
Micro_Organism/Paramecium
Micro_Organism/Rod_bacteria
Micro_Organism/Spherical_bacteria
Micro_Organism/Spiral_bacteria
Micro_Organism/Yeast
</pre>

## Project Structure

The project contains several Jupyter Notebook files. Each notebook implements a different model or set of parameters for the CNN:

| Notebook | Description |
|----------|-------------|
| first_attempt.ipynb | Playground notebook for exploring PyTorch. |
| image_classification[1-4].ipynb | Implementations of a CNN without residual connections, with varying learning rates (0.001 or 0.01) and batch sizes (16 or 32). |
| image_classification[5-8].ipynb | Implementations of a CNN with residual connections, with varying learning rates (0.001 or 0.01) and batch sizes (16 or 32). |
| image_classification_dropout[1-4].ipynb | Implementations of the CNN from image_classification.ipynb with dropout rates from 0.1 to 0.8. |
| image_classification_7_dropout[1-4].ipynb | Implementations of the CNN from image_classification7.ipynb with dropout rates from 0.1 to 0.8. |
| part2/resnet.ipynb | Implementation of transfer learning with the ResNet-18 model, training only the FC layer. |
| part2/resnet2.ipynb | Implementation of transfer learning with the ResNet-18 model, training the last two convolutional layers and the FC layer. |

## Usage

1. Install the required Python version and the **`torch`**, **`torchvision`**, **`torchaudio`** packages.
2. Download and arrange the folder structure for Micro_Organism dataset as described above.
3. Run the desired notebook(s) to train and evaluate the CNN models.
