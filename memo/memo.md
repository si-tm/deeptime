## 試したこと
### 2022/06/29
**[example1](../vampnet/examples/1D_double_well.ipynb)を実行する**  
```import vampnet```  
```ModuleNotFoundError: No module named 'vampnet'```  
がうまく行かない。
1. ```vampnet/```下で、
```bash
python setup.py install
```
2. terminalで
```bash
# Requires the latest pip
pip install --upgrade pip

# Current stable release for CPU and GPU
pip install tensorflow

# Or try the preview build (unstable)
pip install tf-nightly
```
を実行
3. ```pip install vampnet```をファイル内で実行
```
ERROR: Could not find a version that satisfies the requirement vampnet (from versions: none)
ERROR: No matching distribution found for vampnet
WARNING: You are using pip version 20.1.1; however, version 22.1.2 is available.
You should consider upgrading via the '/usr/local/bin/python3.8 -m pip install --upgrade pip' command.
Note: you may need to restart the kernel to use updated packages.
```
```
'/usr/local/bin/python3.8 -m pip install --upgrade pip'
```
をターミナルで実行
```
ERROR: Could not find a version that satisfies the requirement vampnet (from versions: none)
ERROR: No matching distribution found for vampnet
Note: you may need to restart the kernel to use updated packages.
```
[pythonライブラリバージョン問題](https://kajindowsxp.com/pip-unable/)

3. [ここ](../vampnet/README.md)を実行
```
The examples are jupyter notebooks, so the jupyter package is needed to run them:

http://jupyter.readthedocs.io/en/latest/install.html

This is not needed if you'd like to use the package only.

If you want to run the alanine dipeptide example, you'll also need to install the mdshare package (necessary for the download of the trajectory files):

git clone https://github.com/markovmodel/mdshare.git pip install ./mdshare
```

```
Successfully installed humanfriendly-10.0 mdshare-0.4.2
```
