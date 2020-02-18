# Anaconda-Configuration
Kumpulan syntax konfigurasi anaconda install-uninstall-upgrade etc
- [x] Platform Windows 10
- [x] X64 - 64bit
- [x] Connected to the Internet, not using a proxy

# **Install Keras:**
Referensi: [Keras.io](https://keras.io/) 

**Tahap 1**, periksa apakah python, pip dan virtualenv sudah terinstall, eksekusi masing-masing (*anaconda prompt*):
~~~
python --version
pip --version
virtualenv --version
~~~
Upgrade pip ke versi terbaru (*anaconda prompt*)
~~~
python -m pip install --upgrade pip
~~~
Install virtualenv, jika belum ada (*anaconda prompt*)
~~~
pip install virtualenv
~~~
**Tahap 2**, install Tensorflow (*anaconda prompt*)
Referensi: Instalasi [Tensorflow](https://www.tensorflow.org/install/pip).
~~~
pip install tensorflow
~~~
**Tahap 3**, install Microsoft Visual C++ Redistributable for Visual Studio 2019 (or latest year). Download installer di [Visual Studio Microsoft](https://visualstudio.microsoft.com/downloads/). *Other tools and framework* section

**Tahap 4**, periksa apakah tensorflow sudah terinstall (*anaconda prompt*, masuk ke python >>)
~~~
python
import tensorflow as tf
tf.__version__
~~~

**Tahap 5**, install Keras (*anaconda prompt*)
~~~
pip install keras
~~~

# Install CUDA (untuk NVIDIA GPU)

1. Install [CUDA Toolkit](https://developer.nvidia.com/cuda-downloads)
2. Install [CuDNN](https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html)

# **Modul-modul lain sesuai kebutuhan (antara lain):**

Update Anaconda (*anaconda prompt*)
~~~
conda update anaconda
~~~
Install TorchText (*anaconda prompt*):
~~~
conda install -c pytorch torchtext
~~~
Install pydot (*anaconda prompt*)
~~~
pip install pydot
~~~
