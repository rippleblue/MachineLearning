# K-means
```
sudo apt install -y python-dev python-pip python-nose gcc g++ git gfortran vim
sudo apt install -y libopenblas-dev liblapack-dev libatlas-base-dev
apt install build-essential
apt install python-dev
pip install numpy
pip install scipy
pip install -U scikit-learn
```
```
from sklearn import datasets
from sklearn.cluster import KMeans
import numpy as np
iris = datasets.load_iris()
X = iris.data[:, :2] 
y_pred = KMeans(n_clusters=3).fit_predict(X)
for n,a in zip(list(X),list(y_pred)):
    print (n,a)
```
