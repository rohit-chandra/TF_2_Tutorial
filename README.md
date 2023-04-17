# TF_2_Tutorial

**Tensorflow installation instructions on windows native:**

Tutorial link: https://www.youtube.com/watch?v=hHWkvEcDBO0&t=366s

**Note:** Caution: TensorFlow 2.10 was the last TensorFlow release that supported GPU on native-Windows. Starting with TensorFlow 2.11, you will need to install TensorFlow in WSL2, or install tensorflow-cpu and, optionally, try the TensorFlow-DirectML-Plugin

link: https://www.tensorflow.org/install/pip#windows-native

```conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0
# Anything above 2.10 is not supported on the GPU on Windows Native
python -m pip install "tensorflow<2.11"
# Verify install:
python -c "import tensorflow as tf; print(tf.config.list_physical_devices('GPU'))"
```