# Satellite-Imagery
Linear Feature Extraction in Satellite Imagery

Approach
I developed a deep learning model using the U-Net architecture to extract road networks from satellite images. Since separate mask directories were not provided, I generated masks by converting images to grayscale and applying a threshold. The model was trained on these generated masks and validated on a separate dataset.

Model Architecture
The U-Net model consists of:
Contracting Path (Encoder): Captures contextual features by downsampling the image.
Bottleneck: Serves as a bridge between the encoder and decoder.
Expansive Path (Decoder): Upsamples and combines features from the encoder to reconstruct the segmentation map.
Output Layer: Produces a binary mask to identify road pixels.

Results
The model demonstrated effective road network extraction, with good validation accuracy. The visualizations of predictions showed the model's capability to accurately segment roads from satellite imagery.

Conclusion
I successfully used the U-Net model to handle the task of road extraction from satellite images, proving its applicability in real-world scenarios like disaster response and mapping. Further improvements could include fine-tuning and using more advanced models.
