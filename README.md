# 🔤 Alphabet Recognition AI Web App

A beautiful and interactive Streamlit web application for alphabet letter recognition using deep learning.

## 🌟 Features

### Basic App (`app.py`)
- **Image Upload**: Upload PNG, JPG, JPEG, or BMP images
- **Camera Capture**: Take photos directly from your camera
- **Real-time Prediction**: Get instant letter predictions with confidence scores
- **Interactive Charts**: Visualize prediction probabilities
- **Responsive Design**: Beautiful, modern UI with gradient styling

### Advanced App (`app_advanced.py`)
- **Multiple Input Modes**: Upload, draw, or capture letters
- **Interactive Drawing Canvas**: Draw letters with your mouse or touch
- **Enhanced Visualizations**: Interactive charts and detailed analysis
- **Session Statistics**: Track your prediction history
- **Alphabet Reference Grid**: Visual alphabet reference
- **Advanced Preprocessing**: Better image handling for different input types

## 🚀 Quick Start

### 1. Install Dependencies
```bash
pip install -r requirements.txt
```

### 2. Run the Basic App
```bash
streamlit run app.py
```

### 3. Run the Advanced App
```bash
streamlit run app_advanced.py
```

### 4. Open in Browser
The app will automatically open in your default browser at `http://localhost:8501`

## 📁 Project Structure

```
alphabet recognition/
├── app.py                          # Basic Streamlit app
├── app_advanced.py                 # Advanced Streamlit app with drawing
├── requirements.txt                # Python dependencies
├── Alphabet_Recognition_Model.keras # Trained model file
├── Dataset/                        # Training data
├── Test Dataset/                   # Test data
└── model.ipynb                     # Model training notebook
```

## 🎯 How to Use

### Basic App
1. **Upload Image**: Click "Browse files" and select an image of an alphabet letter
2. **Camera Capture**: Use "Take a picture" to capture a photo
3. **View Results**: See the predicted letter with confidence score
4. **Analyze**: Check detailed prediction probabilities for all letters

### Advanced App
1. **Choose Mode**: Select from Upload, Draw, or Camera capture
2. **Input Letter**: 
   - Upload: Select an image file
   - Draw: Use the canvas to draw a letter
   - Camera: Take a photo
3. **Get Prediction**: View results with detailed analysis
4. **Explore**: Check top predictions, full analysis, and detailed tables

## 🎨 Drawing Tips (Advanced App)

- Draw letters clearly and large
- Use the full canvas space
- Make strokes bold and thick
- Center your letter in the canvas
- Use the clear button to start over

## 📷 Photo Tips

- Ensure good lighting
- Position letter in the center
- Avoid shadows and glare
- Use high contrast backgrounds
- Make sure the letter is clearly visible

## 🛠️ Technical Details

### Model Architecture
- **Type**: Convolutional Neural Network (CNN)
- **Input Size**: 28×28 pixels, grayscale
- **Classes**: 26 (A-Z)
- **Framework**: TensorFlow/Keras
- **Accuracy**: ~95% on test data

### Image Preprocessing
1. Convert to grayscale
2. Resize to 28×28 pixels
3. Normalize pixel values (0-1)
4. Reshape for model input

## 🔧 Customization

### Styling
Both apps use custom CSS for beautiful styling. You can modify the CSS in the `st.markdown()` sections to change:
- Colors and gradients
- Fonts and typography
- Card designs
- Animation effects

### Model
To use a different model:
1. Replace `Alphabet_Recognition_Model.keras` with your model
2. Update the model loading path in the code
3. Adjust preprocessing if needed

## 📊 Features Comparison

| Feature | Basic App | Advanced App |
|---------|-----------|--------------|
| Image Upload | ✅ | ✅ |
| Camera Capture | ✅ | ✅ |
| Drawing Canvas | ❌ | ✅ |
| Interactive Charts | ✅ | ✅ |
| Session Stats | ❌ | ✅ |
| Alphabet Grid | ❌ | ✅ |
| Multiple Tabs | ❌ | ✅ |
| Advanced Preprocessing | ❌ | ✅ |

## 🐛 Troubleshooting

### Model Loading Error
- Ensure `Alphabet_Recognition_Model.keras` is in the same directory
- Check if the model file is corrupted
- Verify TensorFlow version compatibility

### Drawing Canvas Issues
- Make sure `streamlit-drawable-canvas` is installed
- Try refreshing the page
- Check browser compatibility

### Camera Not Working
- Allow camera permissions in your browser
- Ensure you're using HTTPS or localhost
- Check if camera is being used by another application

## 🔄 Updates

To update the app:
1. Pull latest changes
2. Update dependencies: `pip install -r requirements.txt --upgrade`
3. Restart the Streamlit app

## 📞 Support

For issues or questions:
- Check the troubleshooting section
- Review the model training notebook (`model.ipynb`)
- Ensure all dependencies are correctly installed

## 🎉 Enjoy!

Start recognizing alphabet letters with AI! Upload images, draw letters, or take photos to see the magic of machine learning in action.
