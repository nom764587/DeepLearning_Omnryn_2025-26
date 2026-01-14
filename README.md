# DeepLearning_Omnryn_2025-26
10 Object detection function in tensorflow 
tf.keras.utils.get_file or similar: Function used for downloading pre-trained model checkpoint
tf.saved_model.load: Core function to load a pre-trained or fine-tuned object detection model into memory for inference.
tf.image.decode_image: Used for decoding raw image data into a TensorFlow tensor.
tf.image.resize or similar preprocessing: Functions to resize the input image to the dimensions expected by the specific model architecture
tf.expand_dims: A function to add a batch dimension to a single image tensor, as models typically expect a batch of images as input 
model.predict() or calling the model directly: The primary function for running the inference process on the input image tensor to get raw detection outputs.
tf.image.non_max_suppression (NMS): A crucial post-processing function that filters out redundant and overlapping bounding boxes, ensuring only a single, high-confidence box per object instance is kept.
Visualization Helper Functions: Custom helper functions are used to draw the final bounding boxes and labels onto the original image for human interpretation.
model.save(): Function used to save a fine-tuned or newly trained model in the SavedModel format for future deployment. 
