## How to use it
1. Install additional environment for [MCG-NJU/MGSampler](https://github.com/MCG-NJU/MGSampler):  
```
pip install -U scikit-image
pip install ffmpeg-python
```
2. Download the [loading.py](https://github.com/lissa2077/MGSampler/blob/main/loading.py) provided by this project.  
3. Clone original [mmaction2](https://github.com/open-mmlab/mmaction2) project.  
```
git clone https://github.com/open-mmlab/mmaction2
```
4. Aftering cloning, in original mmaction2 folder, replace [mmaction2/mmaction/datasets/pipelines/loading.py](https://github.com/open-mmlab/mmaction2/blob/master/mmaction/datasets/pipelines/loading.py) to the [loading.py](https://github.com/lissa2077/MGSampler/blob/main/loading.py) provided by this project.  
```
rm -rf mmaction2/mmaction/datasets/pipelines/loading.py
cp loading.py mmaction2/mmaction/datasets/pipelines/loading.py
```
5. Go to the mmaction2 folder and install mmaction2 folder with new loading.py.  
If you install original mmaction2 before, please remove the old version and then re-install this new version.
```
cd mmaction2
pip install -r requirements/build.txt
pip install -v -e .  # or "python setup.py develop"
```


## Overview
This is forked from [MCG-NJU/MGSampler](https://github.com/MCG-NJU/MGSampler). Combined its part of changes for easily matching to new version [mmaction2](https://github.com/open-mmlab/mmaction2) in future use.
The git project [MCG-NJU/MGSampler](https://github.com/MCG-NJU/MGSampler) is the implementation of [MGSampler](https://arxiv.org/abs/2104.09952) and its code is based on [mmaction2](https://github.com/open-mmlab/mmaction2).
