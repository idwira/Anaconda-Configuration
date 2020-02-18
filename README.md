# Anaconda-Configuration
Kumpulan syntax konfigurasi anaconda install-uninstall-upgrade etc
- [x] Platform Windows 10
- [x] X64 - 64 Bit

# **Install Keras:**

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

**Modul-modul lain sesuai kebutuhan (antara lain):**

Install TorchText (*anaconda prompt*):
~~~
conda install -c pytorch torchtext
~~~
