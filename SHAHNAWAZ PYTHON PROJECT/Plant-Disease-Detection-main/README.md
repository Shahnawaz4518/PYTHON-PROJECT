# 🌿 Plant Disease Detection

A deep learning-based plant disease detection system that can identify 39 different types of plant diseases using images of plant leaves. The system utilizes Convolutional Neural Networks (CNN) built with PyTorch framework and achieves high accuracy in disease classification.

## 🎯 Key Features

- Detects 39 different categories of plant diseases
- High accuracy (~98.9% on test set)
- User-friendly web interface
- Detailed disease information and treatment suggestions
- Built using PyTorch and Flask
- Real-time disease detection from leaf images

## 🔧 Technical Details

### Model Architecture
- CNN with 4 convolutional blocks (32→64→128→256 channels)
- Each block: 2x Conv layers + ReLU + BatchNorm + MaxPool
- Dense layers: 50,176 → 1024 → 39 classes
- Input size: 224x224x3 RGB images
- Total parameters: 52,595,399

### Performance
- Training Accuracy: 96.7%
- Testing Accuracy: 98.9%
- Validation Accuracy: 98.7%

## 🚀 How to Run

1. **Prerequisites**
   - Python 3.x
   - Virtual Environment (recommended)

2. **Installation**
   ```
   # Create and activate virtual environment (optional but recommended)
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate

   # Install dependencies
   pip install -r requirements.txt
   ```

3. **Running the Application**
   - Go to the `Flask Deployed App` folder
   - Download the pre-trained model `plant_disease_model_1_latest.pt` from [here](https://drive.google.com/drive/folders/1ewJWAiduGuld_9oGSrTuLumg9y62qS6A?usp=share_link)
   - Place the model file in the `Flask Deployed App` folder
   - Run the application:
     ```
     python app.py
     ```

## 📊 Dataset

The model is trained on the Plant Village dataset, which contains thousands of images of healthy and diseased plant leaves. The dataset link is available in the blog post mentioned below.

## 🧪 Testing

- Test images are provided in the `test_images` folder
- Each test image is named according to its disease category
- Use these images to verify the model's performance

## 📚 Resources

- [Detailed Blog Post](https://medium.com/analytics-vidhya/plant-disease-detection-using-convolutional-neural-networks-and-pytorch-87c00c54c88f)
- [Live Demo](https://plant-disease-detection-ai.herokuapp.com/)

## 🤝 Contributing

This is an open-source project and contributions are welcome. To contribute:

1. Fork the repository
2. Create your feature branch
3. Make your changes
   - Improve UI
   - Enhance the deep learning model
   - Add documentation
   - Fix bugs
4. Test your changes thoroughly
5. Create a pull request

Please ensure your code is working and well-tested before submitting a pull request.

## 📸 Application Screenshots

1. **Main Page**: User interface for uploading leaf images
2. **AI Engine**: Disease detection in action
3. **Results Page**: Detailed disease information and treatment suggestions
4. **Supplements Store**: Recommended products and treatments
5. **Contact Page**: Get in touch and support

## 📄 License

This project is open-source and available under standard MIT license.

## ✨ Acknowledgments

- PyTorch team for the deep learning framework
- Plant Village dataset creators
- All contributors to this project
