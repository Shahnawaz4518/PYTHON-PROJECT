# 🌿 Plant Disease Detection System

A deep learning-based system that uses Computer Vision and Neural Networks to identify plant diseases from leaf images, enabling early disease detection and treatment recommendations.

## 🔬 Project Overview

This system can detect 39 different types of plant diseases across various plant species including:
- Apple
- Cherry 
- Corn
- Grape
- Orange
- Peach
- Pepper
- Potato
- Tomato
- And more...

## 🎯 Key Features

- Real-time disease detection from plant leaf images
- 98.9% accuracy on test dataset
- Support for 39 different disease categories
- Detailed disease information and treatment recommendations
- User-friendly web interface
- Fast and efficient processing

## 🛠️ Technical Architecture

### Model Details
- Framework: PyTorch
- Architecture: Custom CNN with 4 convolutional blocks
- Input: 224x224x3 RGB images
- Convolutional layers: 32→64→128→256 channels
- Dense layers: 50,176→1024→39 (classes)
- Total Parameters: 52.6M
- Model Size: ~200MB

### Performance Metrics
- Training Accuracy: 96.7%
- Validation Accuracy: 98.7%
- Test Accuracy: 98.9%
- Input Processing Time: <1 second

### Web Application
- Backend: Flask
- Frontend: HTML/CSS/JavaScript
- Deployment: Heroku compatible

## 🚀 Getting Started

1. Clone the repository:
```bash
git clone https://github.com/your-username/Plant-Disease-Detection.git
```

2. Create a virtual environment and activate it:
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Download the pre-trained model:
   - Get `plant_disease_model_1_latest.pt` from the [model link](https://drive.google.com/drive/folders/1ewJWAiduGuld_9oGSrTuLumg9y62qS6A?usp=share_link)
   - Place it in the `Flask Deployed App` folder

5. Run the application:
```bash
cd "Flask Deployed App"
python app.py
```

## 📊 Dataset

The model is trained on the Plant Village dataset, containing 61,486 images of healthy and diseased plant leaves. Dataset characteristics:
- High-quality RGB images
- Controlled environment photos
- Multiple disease stages
- Various lighting conditions
- 39 different classes

## 🧪 Testing

- Test images are provided in `test_images/` folder
- Images include various diseases and healthy leaves
- Each image is labeled with its actual condition
- Use these images to verify model performance

## 📚 Documentation & Resources

- [Detailed Blog Post](https://medium.com/analytics-vidhya/plant-disease-detection-using-convolutional-neural-networks-and-pytorch-87c00c54c88f)
- [Live Demo](https://plant-disease-detection-ai.herokuapp.com/)
- Model architecture details in `Model/` directory
- Implementation code in `Flask Deployed App/` directory

## 👥 Contributing

Contributions are welcome! Areas for improvement:
1. UI/UX enhancements
2. Model optimization
3. Additional plant species support
4. Mobile application development
5. Documentation improvements

## 📄 License

This project is open-source and available under the MIT License.

## ✨ Acknowledgments

- PyTorch team for the deep learning framework
- Plant Village dataset creators
- All contributors to the project
