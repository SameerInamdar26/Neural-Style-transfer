# Real-Time Arbitrary Neural Style Transfer (AdaIN) with Flask UI

An end-to-end Deep Learning pipeline implementing Arbitrary Style Transfer using Adaptive Instance Normalization (AdaIN). The project includes a complete modular architecture featuring an encoder-decoder network, customizable training scripts, and a production-ready Flask web application for real-time inference.

## 🚀 Key Features
* **Arbitrary Style Transfer:** Stylize any content image using any arbitrary style image in a single forward pass (no optimization required per image).
* **AdaIN Architecture:** Features a pre-trained VGG-19 encoder to extract deep features, an Adaptive Instance Normalization layer to align mean and variance, and a custom decoder trained to reconstruct the stylized image.
* **Modular Pipeline:** Separate decoupled modules for model definitions, custom training workflows, utilities, and deployment.
* **Production Flask UI:** A sleek, user-friendly frontend allowing seamless image uploads, asynchronous stylization processing, and immediate output rendering.

## 📁 Repository Structure
* `app.py` - Main Flask application configuration & server runtime.
* `train.py` - Modular training script supporting argparser for hyperparameters, dynamic checkpoints, and evaluation logging.
* `utils/` - Custom data loaders, image preprocessing transforms, and helper modules.
* `encoder_weights.pth` & `decoder_weights.pth` - Serialized model checkpoints representing the optimized latent space weights.
* `templates/` & `static/` - Frontend HTML templates and asset delivery configurations.

## 🛠️ Tech Stack
* **Deep Learning Framework:** PyTorch, Torchvision
* **Backend Web Server:** Flask (Python)
* **Image Processing:** OpenCV, Pillow (PIL)
* **Environment & Deployment:** Docker, Git