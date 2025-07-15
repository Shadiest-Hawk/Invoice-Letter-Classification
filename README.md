# Invoice & Letter Classification

This project is a simple deep learning pipeline for classifying document images as either **invoice** or **letter** using PyTorch and torchvision. It includes a custom dataset loader, a convolutional neural network, training/testing routines, and prediction utilities.

## How to Use

1. **Prepare the Data**
   - Download the [RVL-CDIP dataset](https://www.kaggle.com/datasets/pdavpoojan/the-rvlcdip-dataset-test).
   - **Extract only the `invoice` and `letter` folders** from the dataset. Place them in:
     ```
     rvl_cdip_subset/images/invoice/
     rvl_cdip_subset/images/letter/
     ```
   - You can also use the provided `demo_data/` for quick testing.

2. **Install Requirements**
   - Install dependencies:
     ```bash
     pip install -r requirements.txt
     ```

3. **Run the Notebook**
   - Open `main.ipynb` in Jupyter or VS Code.
   - Run all cells to train and evaluate the model.
   - The trained model will be saved as `invoice_letter_classifier.pth`.

## Project Structure

- `main.ipynb` — Main notebook for training, testing, and prediction
- `requirements.txt` — Python dependencies
- `invoice_letter_classifier.pth` — Saved model weights
- `demo_data/` — Sample images for quick testing
- `rvl_cdip_subset/images/` — Place extracted `invoice` and `letter` folders here

## Notes
- Only the `invoice` and `letter` folders are needed from the RVL-CDIP dataset for this project.
- The model is a simple CNN and may be improved with more data or advanced architectures.

## License
This project is for educational purposes.
