# Anaconda-Configuration
Kumpulan syntax konfigurasi anaconda install-uninstall-upgrade etc
- [x] Platform Windows 10

**Install Keras:**

Tahap 1, periksa apakah python, pip dan virtualenv sudah terinstall, eksekusi masing-masing (*anaconda prompt*):
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
Tahap 2, install Tensorflow (*anaconda prompt*)
Referensi: Instalasi [Tensorflow](https://www.tensorflow.org/install/pip).
~~~
pip install tensorflow
~~~
**Modul-modul lain sesuai kebutuhan (antara lain):**

Install TorchText (*anaconda prompt*):
~~~
conda install -c pytorch torchtext
~~~
