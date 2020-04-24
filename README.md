# Spot-the-Mask-challenge-3rd-Place
## #All against the COVID-19

<div align="center">
    <img src = "https://pbs.twimg.com/media/EVyYt-IU8AALA3x.jpg" 
     height = "500"
     width = "1000">
</div>

     

## 🗒<span style='color:green'> Description </span>


In a time of concerns about slowing the transmission of COVID-19, increased surveillance combined with AI solutions can improve monitoring and reduce the human effort needed to limit the spread of this disease.

Since the anouncement of a lockdown, generalized in many counntries over the world due to the spread of COVID-19, Zindi community has started a new type of challenges called <span style='color:red'>#ZINDIWEEKENDZ </span>. It is a set of competitions based on data science in order to permit to all the #zindians the development of AI based solutions in order to use their skills for giving their community some technical means and  viable solutions to their community in this biological war.
A challenge is taking place every weekend from April to May 2020.

This hackathon was about predicting whether a person in an image is wearing a face mask or not. It was hosted by [Zindi](https://zindi.africa/hackathons/spot-the-mask-challenge/) and lasted for 3 days (from Thursday 17 April to Sunday 19).  

##  😷<span style='color:green'> The solution </span> 🧠
Our solution is based on the architechture of the well known model <a href="https://pytorch.org/hub/pytorch_vision_densenet/">Densnet</a> and uses the technique of transfer learning to get some learned features form others tasks and use them in this contest to help our custom model to make accurate predictions.

<div align="center">
    <img src = "https://pytorch.org/assets/images/densenet1.png" 
        height = "400"
        width = "800">
</div>

The main framework used to implement the model is <a href="https://pytorch.org/get-started/locally/">Pytorch</a>. Some of us also used [Tensorflow 2.0](https://www.tensorflow.org/), [keras](https://keras.io/) and [scikit-learn](https://scikit-learn.org/stable/) when experimenting.

With this model and with all the others techniques applied, we have been able to get the following results:

<div align='center'>

|set        | loss (log_loss)      | accuracy  |
|-----------|----------------------|-----------|
|training   |0.001918              | 99.242  % |
|test       |0.001099342           | 98.141 %  |

</div>


##  🏌<span style='color:green'> Objective </span>
This hackathon was about predicting whether a person in an image is wearing a face mask or not.

⌛ Timeline : **April 17th 2020 11:59 AM - April 19th 2020 11:59PM**

More details here:
https://zindi.africa/hackathons/spot-the-mask-challenge





## 🌴<span style='color:green'> Repository structure (tree😎)</span>
You must follow this structure when runing the notebook.

|----Data  
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      |--- images.zip  
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      |--- train_labels.csv  
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      |--- sample_sub_v2.csv \
| \
|----Mask Challenge Solution  
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;       |--- Spot_the_mask_challenge.ipynb  
|\
|---- Readme.md  
|---- environment.yml\
|---- requirements.txt  


PS : [Download dataset here](https://zindi.africa/hackathons/spot-the-mask-challenge/data) 

Use `pip install -r requirements.txt` to install all the dependencies before going deep.\
\
If you are facing any issues with installation with `pip` you can use the environment.yml file to create an anaconda environment and then use one of these command lines below to activate it (you need to have anaconda distribution and **pip version 9.0.1** installed first) : 

 ```
 # 1- create the anaconda env and install dependencies
 $ conda env create -f environment.yml
 
 # 2- activate the environment containing the dependencies (pytorch, torchvision, keras, opencv etc...)
$ source activate spot-mask-env 

# or

$ conda activate spot-mask-env

# 3- Verify that the new environment was installed correctly by running:
$ conda list

# (optional) 
$ jupyter-notebook
```
Then you will be able now to use `jupyter-notebook` or your favourite text editor to execute the code and get our final result.
\
You will need a suitable **NVIDIA GPU** and **CUDA Toolkit**(>=9.0) to perfectly run the notebook. 

## Command lines summary

<div align="center">

 |command line                     |                Description                                                |
 |---------------------------------|---------------------------------------------------------------------------|
`pip install -r requirements.txt`  | install all the dependencies listed <br> in the file **requirements.txt** |
| `conda env create -f environment.yml`|Create new virtual environment based on the configuration file **environment.yml**|
| `source activate spot-mask-env ` <br> or <br> `conda activate spot-mask-env`| Activate the virtual env named **spot-mask-env**|
| `conda list`|List aull the packages installed into activated venv|
| `jupyter-notebook`|Launch Jupyter notebook web server|
|

</div>


🚨 **The score you will get after runing the code (about 0.00109) is given by predicting on a portion of the test images (public part). The private test images are owned by the organizers of the challenge. the final leaderboard score has been generated after predicting on the full test set.**


## 🏆<span style='color:green'> Final Leaderbord </span>

🏅**Position**: 3rd / 147  
 🏅**Score**: 0.0226 (LogLoss) 

[See the leaderboard](https://zindi.africa/hackathons/spot-the-mask-challenge/leaderboard)
## 💻<span style='color:green'> Authors </span>

<div align='center'>

| Name           |                     Zindi ID                     |                  Github ID               |
|----------------|--------------------------------------------------|------------------------------------------|
|Muhamed TUO     |[@Nazario😁](https://zindi.africa/users/Nazario)  |[@NazarioR9](https://github.com/NazarioR9)|
| Cédric MANOUAN |[@Zeus😆](https://zindi.africa/users/Zeus)        |[@dric2018](https://github.com/dric2018)  |
|Emmanuel KOUPOH |[@eaedk😂](https://zindi.africa/users/eaedk)      |[@eaedk](https://github.com/eaedk)        |

</div>

```
MIT License

<<<<<<< HEAD
Copyright (c) 2020 TheCIA.
=======
## Final Leaderboard
>>>>>>> 23c9dbce4e880024d23d8a776913ea4b51727263

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```
