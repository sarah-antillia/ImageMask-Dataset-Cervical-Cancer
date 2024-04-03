<h2>ImageMask-Dataset-Cervical-Cancer</h2>

This is a simple tool to generate ImageMask-Dataset for Cervical-Cancer.<br><br>
The original dataset used here has been taken from the following kaggle website:<br>
<b>Cervical Cancer largest dataset (SipakMed)</b><br>
<pre>
https://www.kaggle.com/datasets/prahladmehandiratta/cervical-cancer-largest-dataset-sipakmed
</pre>

<h3>1. Dataset Citation</h3>
<pre>
About Dataset
Please don't forget to upvote if you find this useful.
Context
Cervical cancer is the fourth most common cancer among women in the world, estimated more than 0.53 million 
women are diagnosed in every year but more than 0.28 million women’s lives are taken by cervical cancer 
in every years . Detection of the cervical cancer cell has played a very important role in clinical practice.

Content
The SIPaKMeD Database consists of 4049 images of isolated cells that have been manually cropped from 966 cluster
 cell images of Pap smear slides. These images were acquired through a CCD camera adapted to an optical microscope. 
 The cell images are divided into five categories containing normal, abnormal and benign cells.

Acknowledgements
IEEE International Conference on Image Processing (ICIP) 2018, Athens, Greece, 7-10 October 2018.

Inspiration
CERVICAL Cancer is an increasing health problem and an important cause of mortality in women worldwide. 
Cervical cancer is a cancer is grow in the tissue of the cervix . It is due to the abnormal growth of cell that 
are spread to the other part of the body.
Automatic detection technique are used for cervical abnormality to detect Precancerous cell or cancerous cell 
than no pathologist are required for manually detection process.
</pre>


<pre>
./Cervical-Cancer
├─im_Dyskeratotic
│  └─im_Dyskeratotic
│      └─CROPPED
├─im_Koilocytotic
│  └─im_Koilocytotic
│      └─CROPPED
├─im_Metaplastic
│  └─im_Metaplastic
│      └─CROPPED
├─im_Parabasal
│  └─im_Parabasal
│      └─CROPPED
└─im_Superficial-Intermediate
    └─im_Superficial-Intermediate
        └─CROPPED 
</pre>        
        
<h3>2. Generate ImageMask-Dataset</h3>
Please run the following command to create ImageMask-Dataset from the original  SIPaKMeD Database.<br>
<pre>
>python ImageMaskDatasetGenerator.py
</pre>

This Python script <a href="./ImageMaskDatasetGenerator.py">ImageMaskDatasetGenerator.py</a> will generate the following dataset.<br>

<pre>
./Cervical-Cancer-ImageMask-Dataset-V2
├─test
│  ├─Dyskeratotic
│  │  ├─images
│  │  └─masks
│  ├─Koilocytotic
│  │  ├─images
│  │  └─masks
│  ├─Metaplastic
│  │  ├─images
│  │  └─masks
│  ├─Parabasal
│  │  ├─images
│  │  └─masks
│  └─Superficial-Intermediate
│      ├─images
│      └─masks
├─train
│  ├─Dyskeratotic
│  │  ├─images
│  │  └─masks
│  ├─Koilocytotic
│  │  ├─images
│  │  └─masks
│  ├─Metaplastic
│  │  ├─images
│  │  └─masks
│  ├─Parabasal
│  │  ├─images
│  │  └─masks
│  └─Superficial-Intermediate
│      ├─images
│      └─masks
└─valid
    ├─Dyskeratotic
    │  ├─images
    │  └─masks
    ├─Koilocytotic
    │  ├─images
    │  └─masks
    ├─Metaplastic
    │  ├─images
    │  └─masks
    ├─Parabasal
    │  ├─images
    │  └─masks
    └─Superficial-Intermediate
        ├─images
        └─masks
</pre>

We have uploaded this dataset to the google drive <a href="https://drive.google.com/file/d/1DxqbpP6kxzBSdH9jA0gCp8o_znI6Pd-7/view?usp=sharing">
Cervical-Cancer-ImageMask-Dataset-V2.zip</a>.



        