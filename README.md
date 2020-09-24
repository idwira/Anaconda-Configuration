# Anaconda-Configuration
Kumpulan syntax konfigurasi anaconda install-uninstall-upgrade etc
- [x] Platform Windows 10
- [x] X64 - 64bit
- [x] Connected to the Internet, not using a proxy

**Find your installation’s package cache directory: (*anaconda prompt*)**
~~~
conda info
~~~
Melihat list paket-paket (packages)
~~~
conda list
~~~
Referensi: [Managing Packages](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#viewing-a-list-of-installed-packages)

Melihat Current Working Directory (CWD) ((*anaconda prompt*, masuk ke python >>)
~~~
>>> import os
>>> os.getcwd()
~~~

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
Jika gagal, atau pip terhapus lakukan dengan:
1. Download [get-pip.py](https://bootstrap.pypa.io/get-pip.py)
2. Paste file get-pip.py ke folder kerja anaconda, misal C:\Users\nama_user (nama_user bisa "admin" atau sesuai nama user di PC)
3. Pada anaconda prompt jalankan:
~~~
python get-pip.py --user
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
Jika gagal, coba tambahkan "--user" sebagai berikut:
~~~
pip install --user tensorflow
~~~

**Tahap 3**, install Microsoft Visual C++ Redistributable for Visual Studio 2019 (or latest year). Download installer di [Visual Studio Microsoft](https://visualstudio.microsoft.com/downloads/). *Other tools and framework* section

**Tahap 4**, periksa apakah tensorflow sudah terinstall (*anaconda prompt*, masuk ke python >>)
~~~
python
>> import tensorflow as tf
>> tf.__version__
~~~

**Tahap 5**, install Keras (*anaconda prompt*)
~~~
pip install keras
~~~

**Tahap 6**, periksa apakah keras sudah terinstall (*anaconda prompt*, masuk ke python >>)
~~~
python
>> import keras
>> keras.__version__
~~~

# Install CUDA (untuk NVIDIA GPU)

1. Install [CUDA Toolkit](https://developer.nvidia.com/cuda-downloads)
2. Install [CuDNN](https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html)

# **Modul-modul lain sesuai kebutuhan (antara lain):**

Update Anaconda (*anaconda prompt*)
~~~
conda update anaconda
~~~
Install Popular NLTK Data (*anaconda prompt*)
~~~
python -m nltk.downloader popular
~~~
Install [NLTK Data Lainnya](http://www.nltk.org/data.html) (*anaconda prompt*, masuk ke python >>)
~~~
python
>> import nltk
>> nltk.download()
~~~
Install TorchText (*anaconda prompt*):
~~~
conda install -c pytorch torchtext
~~~
Install Pydot (*anaconda prompt*)
~~~
pip install pydot
~~~
Install spaCy (*anaconda prompt*), core large (lg) size around 850 mb
~~~
pip install -U spacy
pip install -U spacy-lookups-data
python -m spacy download en_core_web_lg
~~~
