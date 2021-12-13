# Scene Text Recognition Resources
[<p align='right'>Author: 陈晓雪</p>](https://github.com/CCchenxiaoxue)
The paper "Text Recognition in the Wild: A Survey" (accepted to appear in ACM Computing Surveys) in [arXiv](https://arxiv.org/pdf/2005.03492v3.pdf) version is available now.

### ❗❗ Newest Version Can be Found Here ❗❗
#### This repository is no longer maintaining now, you can refer to our newest one**
##### [Scene Text Recognition Recommendations](https://github.com/HCIILAB/Scene-Text-Recognition-Recommendations)

## Updates

Dec 24, 2019: add 20 papers and update corresponding tables. 

Feb 29, 2020: add AAAI-2020 papers and update corresponding tables. 

May 8, 2020: add CVPR-2020 papers and update corresponding tables. 

Dec 8, 2020: add 11 papers and update corresponding tables. You can download the new [Excel](https://pan.baidu.com/s/1xitxu7R5hw27pVV7eJ1c7w) prepared by us. (Password: sj2t)

***

<!-- MarkdownTOC -->

- [1. Datasets](#1-datasets)
  - [1.1 Regular Latin Datasets](#11-regular-latin-datasets)
  - [1.2 Irregular Latin Datasets](#12-irregular-latin-datasets)
  - [1.3 Multilingual Datasets](#13-multilingual-datasets)
  - [1.4 Synthetic Datasets](#14-synthetic-datasets)
  - [1.5 Comparison of the Benchmark Datasets](#15-comparison-of-the-benchmark-datasets)
- [2. Performance Comparison of Recognition Algorithms](#2-performance-comparison-of-recognition-algorithms)
  - [2.1 Characteristics Comparison of Recognition Approaches](#21-characteristics-comparison-of-recognition-approaches)
  - [2.2 Performance Comparison on Benchmark Datasets](#22-performance-comparison-on-benchmark-datasets)
       - [2.2.1 Performance Comparison of Recognition Algorithms on Regular Latin Datasets](#221-performance-comparison-of-recognition-algorithms-on-regular-latin-datasets)
       - [2.2.2 Performance Comparison of Recognition Algorithms on Irregular Latin Datasets](#222-performance-comparison-of-recognition-algorithms-on-irregular-latin-datasets)
- [3. Survey](#3-survey)
- [4. OCR Service](#4-ocr-service)
- [5. References](#5-references)
- [6.Help](#6help)
- [7.Copyright](#7copyright)

<!-- /MarkdownTOC -->

<a id="1-datasets"></a>
## 1. Datasets

<a id="11-regular-latin-datasets"></a>
### 1.1 Regular Latin Datasets

- IIIT5K[31]：
  * **Introduction:**  The IIIT5K dataset [31] contains 5,000 text instance images: 2,000 for training and 3,000 for testing. It contains words from street scenes and from originally-digital images. Every image is associated with a 50 -word lexicon and a 1,000 -word lexicon. Specifically, the lexicon consists of a ground-truth word and some randomly picked words.
  * **Link:** [IIIT5K-download](http://cvit.iiit.ac.in/research/projects/cvit-projects/the-iiit-5k-word-dataset)
- SVT[1]：
  * **Introduction:**  The SVT dataset [1] contains 350 images: 100 for training and 250 for testing. Some images are severely corrupted by noise, blur, and low resolution. Each image is associated with a 50 -word lexicon.
  * **Link:** [SVT-download](http://vision.ucsd.edu/~kai/svt/)
- ICDAR 2003(IC03)[33]：
  * **Introduction:**  The IC03 dataset [33] contains 509 images: 258 for training and 251 for testing. Specifically, it contains 867 cropped text instances after discarding images that contain non-alphanumeric characters or less than three characters. Every image is associated with a 50 -word lexicon and a full-word lexicon. Moreover, the full lexicon combines all lexicon words.
  * **Link:** [IC03-download](http://www.iapr-tc11.org/mediawiki/index.php?title=ICDAR_2003_Robust_Reading_Competitions)
- ICDAR 2013(IC13)[34]：
  * **Introduction:**  The IC13 dataset [34] contains 561 images: 420 for training and 141 for testing. It inherits data from the IC03 dataset and extends it with new images. Similar to IC03 dataset, the IC13 dataset contains 1,015 cropped text instance images after removing the words with non-alphanumeric characters. No lexicon is associated with IC13 . Notably, 215 duplicate text instance images [65] exist between the IC03 training dataset and the IC13 testing dataset. Therefore, care should be taken regarding the overlapping data when evaluating a model on the IC13 testing data. 
  * **Link:** [IC13-download](http://dagdata.cvc.uab.es/icdar2013competition/?ch=2&com=downloads)
- SVHN[45]：
  * **Introduction:** The SVHN [45] dataset contains more than 600,000 digits of house numbers in natural scenes. It is obtained from a large number of street view images using a combination of automated algorithms and the Amazon Mechanical Turk (AMT) framework. The SVHN dataset was typically  used for scene digit recognition.  
  * **Link:** [SVHN-download](http://ufldl.stanford.edu/housenumbers/)

<a id="12-irregular-latin-datasets"></a>
### 1.2 Irregular Latin Datasets

- SVT-P[35]：
  - **Introduction:** The SVT-P [35] dataset contains 238 images with 639 cropped text instances. It is specifically designed to evaluate perspective distorted text recognition. It is built based on the original SVT dataset by selecting the images at the same address on Google Street View but with different view angles. Therefore, most text instances are heavily distorted by the non-frontal view angle. Moreover, each image is associated with a 50-word lexicon and a full-word lexicon.  
  - **Link:** [SVT-P-download](https://pan.baidu.com/s/1rhYUn1mIo8OZQEGUZ9Nmrg )  \(Password : vnis)
- CUTE80[36]：
  - **Introduction:**  The CUTE80 dataset [36] contains 80 high-resolution images with 288 cropped text
    instances. It focuses on curved text recognition. Most images in CUTE80 have a complex background, perspective distortion, and poor resolution. No lexicon is associated with CUTE80.
  - **Link:** [CUTE80-download](http://cs-chan.com/downloads_CUTE80_dataset.html)
- ICDAR 2015(IC15)[37]：
  - **Introduction:** The IC15 dataset [37] contains 1,500 images: 1,000 for training and 500 for testing.
    Specifically, it contains 2,077 cropped text instances, including more than 200 irregular text samples. As text images were taken by Google Glasses without ensuring the image quality, most of the text is very small, blurred, and multi-oriented. No lexicon is provided.
  - **Link:** [IC15-download](http://rrc.cvc.uab.es/?ch=4&com=downloads)
- COCO-Text[38]：
  - **Introduction:** The COCO-Text dataset [38] contains 63,686 images with 145,859 cropped text instances. It is the first large-scale dataset for text in natural images and also the first dataset to annotate scene text with attributes such as legibility and type of text. However, no lexicon is associated with COCO-Text.  
  - **Link:** [COCO-Text-download](https://vision.cornell.edu/se3/coco-text-2/)
- Total-Text[39]：
  - **Introduction:** The Total-Text dataset [39] contains 1,555 images with 11,459 cropped text instance images. It focuses on curved scene text recognition. Images in Total-Text have more than three different orientations, including horizontal, multi-oriented, and curved. No lexicon is associated with Total-Text.
  - **Link:** [Total-Text-download](https://github.com/cs-chan/Total-Text-Dataset)

<a id="13-multilingual-datasets"></a>
### 1.3 Multilingual Datasets

- RCTW-17(RCTW competition，ICDAR17)[40]：
  - **Introduction:** The RCTW-17 dataset contains 12,514 images: 11,514 for training and 1,000 for testing. Most are natural images collected by cameras or mobile phones, whereas others are digital-born. Text instances are annotated with labels, fonts, languages, etc.    
  - **Link:** [RCTW-17-download](http://rctw.vlrlab.net/dataset/)
- MTWI(competition)[41]：
  - **Introduction:** The MTWI dataset contains 20,000 images. This is the first dataset constructed by Chinese and Latin web text. Most images in MTWI have a relatively high resolution and cover diverse types of web text, including multi-oriented text, tightly-stacked text, and complex-shaped text.  
  - **Link:** [MTWI-download ](https://pan.baidu.com/s/1SUODaOzV7YOPkrun0xSz6A#list/path=%2F)  \(Password:gox9)
- CTW[42]：
  - **Introduction:** The CTW dataset includes 32,285 high-resolution street view images with 1,018,402 character instances. All images have character-level annotations: the underlying character, the bounding box, and six other attributes.
  - **Link:** [CTW-download](https://ctwdataset.github.io/)
- SCUT-CTW1500[43]：
  - **Introduction:** The SCUT-CTW1500 dataset contains 1,500 images: 1,000 for training and 500
    for testing. In particular, it provides 10,751 cropped text instance images, including 3,530 with curved text. The images are manually harvested from the Internet, image libraries such as Google Open-Image, or phone cameras. The dataset contains a lot of horizontal and multi-oriented text   
  - **Link:** [SCUT-CTW1500-download](https://github.com/Yuliang-Liu/Curve-Text-Detector)
* LSVT(LSVT competition, ICDAR2019)[57]:
  * **Introduction:** The LSVT dataset contains 20,000 testing samples, 30,000 fully annotated training samples, and 400,000 training samples with weak annotations (i.e., with partial labels). All images are captured from streets and reflect a large variety of complicated real-world scenarios, e.g., store fronts and landmarks.  
  * **Link:** [LSVT-download](https://rrc.cvc.uab.es/?ch=16&com=downloads)
* ArT(ArT competition, ICDAR2019)[58]:
  * **Introduction:** The ArT dataset [58] contains 10,166 images: 5,603 for training and 4,563 for testing. ArT is a combination of Total-Text, SCUT-CTW 1500 , and Baidu Curved Scene Text 4 , which was collected to introduce the arbitrary-shaped text problem. Moreover, all existing text shapes (i.e., horizontal, multi-oriented, and curved) have multiple occurrences in the ArT dataset.
  * **Link:** [ArT-download](https://rrc.cvc.uab.es/?ch=16&com=downloads)
* ReCTS-25k(ReCTS competition, ICDAR2019)[59]:
  * **Introduction:** The ReCTS-25k dataset [59] contains 25,000 images: 20,000 for training and 5,000 for testing.  All the images are from the Meituan-Dianping Group, collected by Meituan business mer-
    chants, using phone cameras under uncontrolled conditions. Specifically, ReCTS-25 k dataset mainly contains images of Chinese text on signboards.
  * **Link:** [ReCTS-download](https://rrc.cvc.uab.es/?ch=16&com=downloads)
* MLT(MLTcompetition, ICDAR2019) [81]:
  * **Introduction:** The MLT-2019 dataset [81] contains 20,000 images: 10,000 for training (1,000 per language) and 10,000 for testing. The dataset includes ten languages, representing seven different scripts: Arabic, Bangla, Chinese, Devanagari, English, French, German, Italian, Japanese, and Korean. The number of images per script is equal.  
  * **Link:** [MLT-download](https://rrc.cvc.uab.es/?ch=15&com=downloads)  

<a id="14-synthetic-datasets"></a>
### 1.4 Synthetic Datasets

* Synth90k [53] : 
  * **Introduction:** The Synth90k dataset contains 9 million synthetic text instance images from a set of 90k common English words. Words are rendered onto natural images with random transformations and effects, such as random fonts, colors, blur, and noises. Synth90k dataset can emulate the distribution of scene text images and can be used instead of real-world data to train data-hungry deep learning algorithms. Besides, every image is annotated with a ground-truth word.  
  * **Link:** [Synth90k-download](http://www.robots.ox.ac.uk/~vgg/data/text/)
* SynthText [54] : 
  * **Introduction:** The SynthText dataset contains 800,000 images with 6 million synthetic text instances. As in the generation of Synth90k dataset, the text sample is rendered using a randomly selected font and transformed according to the local surface orientation. Moreover, each image is annotated with a ground-truth word.  
  * **Link:** [SynthText-download](https://github.com/ankush-me/SynthText)
* Verisimilar Synthesis [73] : 
  * **Introduction:** The Verisimilar Synthesis dataset [73] contains 5 million synthetic text instance images. Given background images and source texts, a semantic map and a saliency map are first
    determined which are then combined to identify semantically sensible and apt locations for text embedding. The color, brightness, and orientation of the source texts are further determined adaptively according to the color, brightness, and contextual structures around the embedding locations within the background image.  
  * **Link:** [Verisimilar Synthesis](https://github.com/fnzhan/Verisimilar-Image-Synthesis-for-Accurate-Detection-and-Recognition-of-Texts-in-Scenes)
* UnrealText [88]:
  * **Introduction:** The UnrealText dataset [88] contains 600K synthetic images with 12 million cropped text instances. It is developed upon Unreal Engine 4 and the UnrealCV plugin [89]. Text instances are regarded as planar polygon meshes with text foregrounds loaded as texture. These meshes are placed in suitable positions in 3D world, and rendered together with the scene as a whole. The same font set from [Google Fonts](https://fonts.google.com/) and the same text corpus, i.e., Newsgroup20, are used as SynthText does.    
  * **Link:** [Verisimilar Synthesis](https://github.com/fnzhan/Verisimilar-Image-Synthesis-for-Accurate-Detection-and-Recognition-of-Texts-in-Scenes)

<a id="15-comparison-of-the-benchmark-datasets"></a>
### 1.5 Comparison of the Benchmark Datasets

<table cellspacing="0" border="0">
  <colgroup width="271"></colgroup>
  <colgroup width="179"></colgroup>
  <colgroup width="89"></colgroup>
  <colgroup width="122"></colgroup>
  <colgroup width="127"></colgroup>
  <colgroup width="89"></colgroup>
  <colgroup width="179"></colgroup>
  <colgroup width="177"></colgroup>
  <colgroup span="7" width="89"></colgroup>
  <tr>
    <td colspan=15 height="34" align="center"><b>Comparison of the Benchmark Datasets</b></td>
    </tr>
  <tr>
    <td rowspan=2 height="39" align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Datasets&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">Language</td>
    <td colspan=6 align="center">Images</td>
    <td colspan=4 align="center">Lexicon</td>
    <td colspan=2 align="center">Label</td>
    <td rowspan=2 align="center">Type</td>
  </tr>
  <tr>
    <td align="center">Pictures</td>
    <td align="center">Training Pictures</td>
    <td align="center">Testing Pictures</td>
    <td align="center">Instances</td>
    <td align="center">Training Instances</td>
    <td align="center">Testing Instances</td>
    <td align="center" sdval="50" sdnum="2052;">50</td>
    <td align="center">1k</td>
    <td align="center">Full</td>
    <td align="center">None</td>
    <td align="center">Char</td>
    <td align="center">Word</td>
    </tr>
  <tr>
    <td height="20" align="center">IIIT5K[31]</td>
    <td align="center">English</td>
    <td align="center" sdval="1120" sdnum="2052;">1120</td>
    <td align="center" sdval="380" sdnum="2052;">380</td>
    <td align="center" sdval="740" sdnum="2052;">740</td>
    <td align="center" sdval="5000" sdnum="2052;">5000</td>
    <td align="center" sdval="2000" sdnum="2052;">2000</td>
    <td align="center" sdval="3000" sdnum="2052;">3000</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">SVT[32]</td>
    <td align="center">English</td>
    <td align="center" sdval="350" sdnum="2052;">350</td>
    <td align="center" sdval="100" sdnum="2052;">100</td>
    <td align="center" sdval="250" sdnum="2052;">250</td>
    <td align="center" sdval="725" sdnum="2052;">725</td>
    <td align="center" sdval="211" sdnum="2052;">211</td>
    <td align="center" sdval="514" sdnum="2052;">514</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">IC03[33]</td>
    <td align="center">English</td>
    <td align="center" sdval="509" sdnum="2052;">509</td>
    <td align="center" sdval="258" sdnum="2052;">258</td>
    <td align="center" sdval="251" sdnum="2052;">251</td>
    <td align="center" sdval="2268" sdnum="2052;">2268</td>
    <td align="center" sdval="1157" sdnum="2052;">1157</td>
    <td align="center" sdval="1111" sdnum="2052;">1111</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">IC13[34]</td>
    <td align="center">English</td>
    <td align="center" sdval="561" sdnum="2052;">561</td>
    <td align="center" sdval="420" sdnum="2052;">420</td>
    <td align="center" sdval="141" sdnum="2052;">141</td>
    <td align="center" sdval="5003" sdnum="2052;">5003</td>
    <td align="center" sdval="3564" sdnum="2052;">3564</td>
    <td align="center" sdval="1439" sdnum="2052;">1439</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">SVHN[45]</td>
    <td align="center">Digits</td>
    <td align="center" sdval="600000" sdnum="2052;">600000</td>
    <td align="center" sdval="573968" sdnum="2052;">573968</td>
    <td align="center" sdval="26032" sdnum="2052;">26032</td>
    <td align="center" sdval="600000" sdnum="2052;">600000</td>
    <td align="center" sdval="573968" sdnum="2052;">573968</td>
    <td align="center" sdval="26032" sdnum="2052;">26032</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">SVT-P[35]</td>
    <td align="center">English</td>
    <td align="center" sdval="238" sdnum="2052;">238</td>
    <td align="center" sdval="0" sdnum="2052;">0</td>
    <td align="center" sdval="238" sdnum="2052;">238</td>
    <td align="center" sdval="639" sdnum="2052;">639</td>
    <td align="center" sdval="0" sdnum="2052;">0</td>
    <td align="center" sdval="639" sdnum="2052;">639</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">CUTE80[36]</td>
    <td align="center">English</td>
    <td align="center" sdval="80" sdnum="2052;">80</td>
    <td align="center" sdval="0" sdnum="2052;">0</td>
    <td align="center" sdval="80" sdnum="2052;">80</td>
    <td align="center" sdval="288" sdnum="2052;">288</td>
    <td align="center" sdval="0" sdnum="2052;">0</td>
    <td align="center" sdval="288" sdnum="2052;">288</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">IC15[37]</td>
    <td align="center">English</td>
    <td align="center" sdval="1500" sdnum="2052;">1500</td>
    <td align="center" sdval="1000" sdnum="2052;">1000</td>
    <td align="center" sdval="500" sdnum="2052;">500</td>
    <td align="center" sdval="6545" sdnum="2052;">6545</td>
    <td align="center" sdval="4468" sdnum="2052;">4468</td>
    <td align="center" sdval="2077" sdnum="2052;">2077</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">COCO-Text[38]</td>
    <td align="center">English</td>
    <td align="center" sdval="63686" sdnum="2052;">63686</td>
    <td align="center" sdval="43686" sdnum="2052;">43686</td>
    <td align="center" sdval="10000" sdnum="2052;">10000</td>
    <td align="center" sdval="145859" sdnum="2052;">145859</td>
    <td align="center" sdval="118309" sdnum="2052;">118309</td>
    <td align="center" sdval="27550" sdnum="2052;">27550</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">Total-Text[39]</td>
    <td align="center">English</td>
    <td align="center" sdval="1555" sdnum="2052;">1555</td>
    <td align="center" sdval="1255" sdnum="2052;">1255</td>
    <td align="center" sdval="300" sdnum="2052;">300</td>
    <td align="center" sdval="11459" sdnum="2052;">11459</td>
    <td align="center" sdval="11166" sdnum="2052;">11166</td>
    <td align="center" sdval="293" sdnum="2052;">293</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">RCTW-17[40]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="12514" sdnum="2052;">12514</td>
    <td align="center" sdval="11514" sdnum="2052;">11514</td>
    <td align="center" sdval="1000" sdnum="2052;">1000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">MTWI[41]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="20000" sdnum="2052;">20000</td>
    <td align="center" sdval="10000" sdnum="2052;">10000</td>
    <td align="center" sdval="10000" sdnum="2052;">10000</td>
    <td align="center" sdval="290206" sdnum="2052;">290206</td>
    <td align="center" sdval="141476" sdnum="2052;">141476</td>
    <td align="center" sdval="148730" sdnum="2052;">148730</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">CTW[42]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="32285" sdnum="2052;">32285</td>
    <td align="center" sdval="25887" sdnum="2052;">25887</td>
    <td align="center" sdval="3269" sdnum="2052;">3269</td>
    <td align="center" sdval="1018402" sdnum="2052;">1018402</td>
    <td align="center" sdval="812872" sdnum="2052;">812872</td>
    <td align="center" sdval="103519" sdnum="2052;">103519</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">SCUT-CTW1500[43]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="1500" sdnum="2052;">1500</td>
    <td align="center" sdval="1000" sdnum="2052;">1000</td>
    <td align="center" sdval="500" sdnum="2052;">500</td>
    <td align="center" sdval="10751" sdnum="2052;">10751</td>
    <td align="center" sdval="7683" sdnum="2052;">7683</td>
    <td align="center" sdval="3068" sdnum="2052;">3068</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">LSVT[57], [63]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="450000" sdnum="2052;">450000</td>
    <td align="center" sdval="30000" sdnum="2052;">30000</td>
    <td align="center" sdval="20000" sdnum="2052;">20000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">ArT[58]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="10166" sdnum="2052;">10166</td>
    <td align="center" sdval="5603" sdnum="2052;">5603</td>
    <td align="center" sdval="4563" sdnum="2052;">4563</td>
    <td align="center" sdval="98455" sdnum="2052;">98455</td>
    <td align="center" sdval="50029" sdnum="2052;">50029</td>
    <td align="center" sdval="48426" sdnum="2052;">48426</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">ReCTS-25k[59]</td>
    <td align="center">Chinese/English</td>
    <td align="center" sdval="25000" sdnum="2052;">25000</td>
    <td align="center" sdval="20000" sdnum="2052;">20000</td>
    <td align="center" sdval="5000" sdnum="2052;">5000</td>
    <td align="center" sdval="119713" sdnum="2052;">119713</td>
    <td align="center" sdval="108924" sdnum="2052;">108924</td>
    <td align="center" sdval="10789" sdnum="2052;">10789</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">MLT[81]</td>
    <td align="center">Multilingual</td>
    <td align="center" sdval="20000" sdnum="2052;">20000</td>
    <td align="center" sdval="10000" sdnum="2052;">10000</td>
    <td align="center" sdval="10000" sdnum="2052;">10000</td>
    <td align="center" sdval="191639" sdnum="2052;">191639</td>
    <td align="center" sdval="89177" sdnum="2052;">89177</td>
    <td align="center" sdval="102462" sdnum="2052;">102462</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Irregular</td>
  </tr>
  <tr>
    <td height="20" align="center">Synth90k[53]</td>
    <td align="center">English</td>
    <td align="center">~9000000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">~9000000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
  <tr>
    <td height="20" align="center">SynthText[54]</td>
    <td align="center">English</td>
    <td align="center">~6000000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">~6000000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
    <tr>
    <td height="20" align="center">Verisimilar Synthesis[73]</td>
    <td align="center">English</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">~5000000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
    <tr>
    <td height="20" align="center">UnrealText[88]</td>
    <td align="center">English</td>
    <td align="center">~600000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">~12000000</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center"> √</td>
    <td align="center">√</td>
    <td align="center">Regular</td>
  </tr>
</table>

***

<a id="2-performance-comparison-of-recognition-algorithms"></a>
## 2. Performance Comparison of Recognition Algorithms

<a id="21-characteristics-comparison-of-recognition-approaches"></a>
### 2.1 Characteristics Comparison of Recognition Approaches

It is notable that 1) "Reg" stands for regular Latin datasets. 2) "Irreg" stands for irregular Latin datasets. 3) "Seg" denotes the segmentation-based methods. 4) "Extra" indicates the methods that use the extra datasets other than Synth90k and SynthText. 5) "CTC" represents the methods that apply the CTC-based algorithm to decode. 6) "Attn" represents the method that apply the attention mechanism to decode.

You can also download the new [Excel](https://pan.baidu.com/s/1xitxu7R5hw27pVV7eJ1c7w) prepared by us. (Password: sj2t)

<table cellspacing="0" border="0">
  <colgroup width="271"></colgroup>
  <colgroup span="3" width="89"></colgroup>
  <colgroup width="104"></colgroup>
  <colgroup span="3" width="89"></colgroup>
  <colgroup span="2" width="86"></colgroup>
  <colgroup width="832"></colgroup>
  <tr>
    <td colspan=11 height="34" align="center"><b>Characteristics Comparison of Recognition Approaches</b></td>
    </tr>
  <tr>
    <td rowspan=2 height="39" align="center"><b>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Method&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</b></td>
    <td rowspan=2 align="center"><b>Code</b></td>
    <td rowspan=2 align="center"><b>Regular</b></td>
    <td rowspan=2 align="center"><b>Irregular</b></td>
    <td rowspan=2 align="center"><b>Segmentation</b></td>
    <td rowspan=2 align="center"><b>Extra data</b></td>
    <td rowspan=2 align="center"><b>CTC</b></td>
    <td rowspan=2 align="center"><b>Attention</b></td>
    <td rowspan=2 align="center"><b>Source</b></td>
    <td rowspan=2 align="center"><b>Time</b></td>
    <td rowspan=2 align="center"><b>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Highlight&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</b></td>
  </tr>
  <tr>
    </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : ABBYY</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center"> ×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
    <td align="center">a state-of-the-art text detector + a leading commercial OCR engine</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : SYNTH+PLEX</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
    <td align="center">the baseline of scene text recognition</td>
  </tr>
  <tr>
    <td height="20" align="center">Mishra et al. [2]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
    <td align="center">1) incorporating higher order statistical language models to recognize words in an unconstrained manner 2) introducing IIIT5K-word dataset</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [3]</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
    <td align="center">CNNs + Non-maximal suppression + beam search</td>
  </tr>
  <tr>
    <td height="20" align="center">Goel et al. [4] : wDTW</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
    <td align="center">recognizing text by matching the scene and synthetic image features with wDTW</td>
  </tr>
  <tr>
    <td height="20" align="center">Bissacco et al. [5] : PhotoOCR</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
    <td align="center">applying a network with five hidden layers for character classification</td>
  </tr>
  <tr>
    <td height="20" align="center">Phan et al. [6]</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
    <td align="center">1) MSER + SIFT descriptors + SVM 2) introducing the SVT-P datasets</td>
  </tr>
  <tr>
    <td height="20" align="center">Alsharif et al. [7] : HMM/Maxout</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
    <td align="center">convolutional Maxout networks + Hybrid HMM</td>
  </tr>
  <tr>
    <td height="20" align="center">Almazan et al [8] : KCSR</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
    <td align="center">embedding word images and text strings in a common vectorial subspace and interpreting the task of recognition and retrieval as a nearest neighbor problem</td>
  </tr>
  <tr>
    <td height="20" align="center">Yao et al. [9] : Strokelets</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
    <td align="center">proposing a novel multi-scale representation for scene text recognition: strokelets</td>
  </tr>
  <tr>
    <td height="20" align="center">R.-Serrano et al.[10] : Label embedding</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
    <td align="center">embedding word labels and word images into a common Euclidean space and finding the cloest word label in this space</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [11]</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
    <td align="center">1) enabling efficient feature sharing for text detection and classification 2) making technical changes over the traditional CNN architectures 3) proposing a method of automated data mining of Flickr.</td>
  </tr>
  <tr>
    <td height="20" align="center">Su and Lu [12]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">ACCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
    <td align="center">HOG + BLSTM + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Gordo[13] : Mid-features</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
    <td align="center">proposing local mid-level features for building word image representations</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [14]</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
    <td align="center">1) treating each word as a category and training very large convolutional neural networks to perform word recognition on the whole proposal region 2) generating 9 million images with equal numbers of word samples from a 90k word dictionary</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [15]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
    <td align="center">CNN + CRF</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi, Bai, and Yao [16] : CRNN</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">CNN + BLSTM + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [17] : RARE</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
    <td align="center">STN + CNN + attentional BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Lee and Osindero [18] : R2AM</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
    <td align="center">presenting recursive recurrent neural networks with attention modeling</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [19] : STAR-Net</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
    <td align="center">STN + ResNet + BLSTM + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al. [78]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
    <td align="center">integrating the CNN and WFST classification model</td>
  </tr>
  <tr>
    <td height="20" align="center">Mishra et al. [77]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">CVIU</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
    <td align="center">character detection (HOG/CNN + SVM +Sliding window) + CRF, combining bottom-up cues from character detection and top-down cues from lexicon</td>
  </tr>
  <tr>
    <td height="20" align="center">Su and Lu [76]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">PR</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">HOG(different scale) + BLSTM + CTC (ensemble)</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yang et al. [20]</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">IJCAI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">1) CNN + 2D attention-based RNN, applying an auxiliary dense character detection task that helps to learn text specific visual patterns 2) developing a large-scale synthetic dataset</td>
  </tr>
  <tr>
    <td height="20" align="center">Yin et al. [21]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">CNN + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[66] : GRCNN</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">Gated Recurrent Convulution Layer + BLSTM + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">*Cheng et al. [22] : FAN</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
    <td align="center">1) proposing the concept of attention drift 2)introducing focusing network to focus deviated attention back on the target areas</td>
  </tr>
  <tr>
    <td height="20" align="center">Cheng et al. [23] : AON</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">1) extracting scene text features in four directions 2) CNN + Attentional BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [24]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">attentional ResNet + CNN + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [25] : Char-Net</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">CNN + STN (facilitating the rectification of individual characters) + LSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liu et al.  [26] : SqueezedText</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">binary convolutional encoder-decoder network + Bi-RNN</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhan et al.[73]</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">CRNN, achieving verisimilar scene text image synthesis by combining three novel designs, including semantic coherence, visual attention, and adaptive text appearance</td>
  </tr>
  <tr>
    <td height="20" align="center">*Bai et al. [27] : EP</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">proposing edit probability to effectively handle the misalignment between the training text and the output probability distribution sequence</td>
  </tr>
  <tr>
    <td height="20" align="center">Fang et al.[74]</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">MultiMedia</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">ResNet + [2D Attentional CNN, CNN-based language module]</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.[75] : EnEsCTC</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">proposing a novel maximum entropy based regularization for CTC (EnCTC) and an entropy-based pruning method (EsCTC) to effectively reduce the space of the feasible set</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al. [28]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">designing a multi-task network with an encoder-discriminator-generator architecture to guide the feature of the original image toward that of the clean image</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[61] : MAAN</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICFHR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">ResNet + BLSTM + Memory-Augmented attentional decoder</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [29]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">attentional DenseNet + BLSTM + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [30] : ASTER</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
    <td align="center">TPS + ResNet + bidirectional attention-based BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : ASTER + AEG</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">TPS + ResNet + bidirectional attention-based BLSTM + AEG</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [46] : MORAN</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Multi-object rectification network + CNN + attentional BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [61] : MORAN-v2</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Multi-object rectification network + ResNet + attentional BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : MORAN-v2 + AEG</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Multi-object rectification network + ResNet + attentional BLSTM + AEG</td>
  </tr>
  <tr>
    <td height="20" align="center">Xie et al. [47] : CAN</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ACM</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ResNet + CNN + GLU</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liao et al.[48] : CA-FCN</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">performing character classification at each pixel location and needing character-level annotations</td>
  </tr>
  <tr>
    <td height="20" align="center">*Li et al. [49] : SAR</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ResNet + 2D attentional LSTM</td>
  </tr>
  <tr>
    <td height="23" align="center">Zhan el at. [55]: ESIR</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Iterative rectification Network + ResNet + attentional BLSTM</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [56]: SSDAN</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">attentional CNN + GAS + GRU</td>
  </tr>
  <tr>
    <td height="20" align="center">Yang et al. [62]: ScRN</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Symmetry-constrained Rectification Network + ResNet + BLSTM + attentional GRU</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [64]: GCAM</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICME</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Convolutional Block Attention Module (CBAM) + ResNet + BLSTM + the proposed Gated Cascade Attention Module (GCAM)</td>
  </tr>
  <tr>
    <td height="20" align="center">Jeonghun et al. [65]</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">TPS + ResNet + BLSTM + Attention Mechanism</td>
  </tr>
  <tr>
    <td height="20" align="center">Huang et al. [67] : EPAN</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">learning to sample features from the text region of 2D feature maps and innovatively introducing a two-stage attention mechanism</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [68]</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">attentional DenseNET + 4-layer CNN + CTC</td>
  </tr>
  <tr>
    <td height="20" align="center">Qi et al. [69] : CCL</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ResNet + [CTC, CCL]</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [70] : ReELFA</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">VGG + attentional LSTM, utilizing one-hot encoded coordinates to indicate the spatial relationship of pixels and character center masks to help focus attention on the right feature areas</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhu et al. [71] : HATN</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ResNet50 + Hierarchical Attention Mechanism (Transformer structure)</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhan et al. [72] : SF-GAN</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">ResNet50 + attentional Decoder, synthesising realistic scene text images for training better recognition models</td>
  </tr>
  <tr>
    <td height="20" align="center">Liao et al. [79] : SAM</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Spatial attentional module (SAM)</td>
  </tr>
  <tr>
    <td height="20" align="center">Liao et al. [79] : seg-SAM</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">Character segmentation module + Spatial attention module (SAM)</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [80] : DAN</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">decoupling the decoder of the traditional attention mechanism into a convolutional alignment module and a decoupled text decoder</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [82] : TextSR</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
    <td align="center">attempting to solve small texts with super-resolution methods</td>
  </tr>
  <tr>
    <td height="20" align="center">Wan et al. [83] : TextScanner</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">an effective segmentation-based dual-branch framework for scene text recognition</td>
  </tr>
  <tr>
    <td height="20" align="center">Hu et al. [84] : GTC</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">attempting to use GCN to learn the local correlations of feature sequence</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [85] </td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">separating text content from noisy background styles</td>
  </tr>
  <tr>
    <td height="20" align="center">*Litman et al. [86]</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">training a deep BiLSTM encoder, thus improving the encoding of contextual dependencies</td>
  </tr>
  <tr>
    <td height="20" align="center">Yu et al. [87]</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center"> introducing a global semantic reasoning module (GSRM) to capture global semantic context through multi-way parallel transmission</td>
  </tr>
  <tr>
    <td height="20" align="center">Qiao et al. [101] : SEED</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center"> proposing a semantics enhanced encoder-decoder framework to robustly recognize low-quality scene texts</td>
  </tr>
  <tr>
    <td height="20" align="center">Bleeker et al. [93] : Bi-STET</td>
    <td align="center">√</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ECAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">a novel bidirectional STR method with a single decoder for bidirectional text decoding</td>
  </tr>
  <tr>
    <td height="20" align="center">*Bartz et al. [94] : KISS</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">a new model for STR that consists of two ResNet based feature extractors, a spatial transformer, and a transformer</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [95] : SPIN</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">a new learnable geometric-unrelated module which allows the color manipulation of source data within the network</td>
  </tr>
  <tr>
    <td height="20" align="center">Lin et al. [96] : FASDA</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">implementing sequence-level domain adaption for STR</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [98] : AutoSTR</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">searching data-dependent backbones</td>
  </tr>
  <tr>
    <td height="20" align="center">Mou et al. [99] : PlugNet</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center">combining the pluggable super-resolution unit to solve the low-quality text recognition from the feature-level</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yue et al. [100] : RobustScanner</td>
    <td align="center">×</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">×</td>
    <td align="center">√</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
    <td align="center"> mitigating the misrecognition problem of the encoderdecoder with attention framework on contextless text images</td>
  </tr>
</table>

<a id="22-performance-comparison-on-benchmark-datasets"></a>
### 2.2 Performance Comparison on Benchmark Datasets

In this section, we compare the performance of the current advanced algorithms on benchmark datasets, including IIIT5K，SVT，IC03，IC13，SVT-P，CUTE80，IC15，COCO-Text, RCTW-17, MWTI, CTW，SCUT-CTW1500, LSVT, ArT and ReCTS-25k.

It is notable that 1) The '*' indicates the methods that use the extra datasets other than Synth90k and SynthText. 2) The **bold** represents the best recognition results. 3) '^' denotes the best recognition results of using extra datasets. 4) '@' represents the methods under different evaluation that only uses 1811 test images. 5) 'SK', 'ST', 'ExPu', 'ExPr' and 'Un' indicates the methods that use Synth90K, SynthText, Extra Public Data, Extra Private Data and unknown data, respectively. 6) 'D_A' means data augmentation. 7) IC5-S contains only 1811 cropped text instances.

<a id="221-performance-comparison-of-recognition-algorithms-on-regular-latin-datasets"></a>
#### 2.2.1 Performance Comparison of Recognition Algorithms on Regular Latin Datasets

<table cellspacing="0" border="0">
  <colgroup width="271"></colgroup>
  <colgroup span="10" width="89"></colgroup>
  <colgroup width="172"></colgroup>
  <colgroup span="2" width="86"></colgroup>
  <tr>
    <td colspan=14 height="34" align="center"><b>Performance Comparison of Recognition Algorithms on Regular Latin Datasets</b></td>
    </tr>
  <tr>
    <td rowspan=2 height="39" align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Method&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td colspan=3 align="center">IIIT5K</td>
    <td colspan=2 align="center">SVT</td>
    <td colspan=4 align="center">IC03</td>
    <td align="center">IC13</td>
    <td rowspan=2 align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Data&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">Source</td>
    <td rowspan=2 align="center">Time</td>
  </tr>
  <tr>
    <td align="center" sdval="50" sdnum="2052;">50</td>
    <td align="center">1K</td>
    <td align="center">None</td>
    <td align="center" sdval="50" sdnum="2052;">50</td>
    <td align="center">None</td>
    <td align="center" sdval="50" sdnum="2052;">50</td>
    <td align="center">Full</td>
    <td align="center">50k</td>
    <td align="center">None</td>
    <td align="center">None</td>
    </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : ABBYY</td>
    <td align="center" sdval="24.3" sdnum="2052;">24.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="35" sdnum="2052;">35</td>
    <td align="center">-</td>
    <td align="center" sdval="56" sdnum="2052;">56</td>
    <td align="center" sdval="55" sdnum="2052;">55</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">Un</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : SYNTH+PLEX</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="57" sdnum="2052;">57</td>
    <td align="center">-</td>
    <td align="center" sdval="76" sdnum="2052;">76</td>
    <td align="center" sdval="62" sdnum="2052;">62</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
  </tr>
  <tr>
    <td height="20" align="center">Mishra et al. [2]</td>
    <td align="center" sdval="64.1" sdnum="2052;">64.1</td>
    <td align="center" sdval="57.5" sdnum="2052;">57.5</td>
    <td align="center">-</td>
    <td align="center" sdval="73.2" sdnum="2052;">73.2</td>
    <td align="center">-</td>
    <td align="center" sdval="81.8" sdnum="2052;">81.8</td>
    <td align="center" sdval="67.8" sdnum="2052;">67.8</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [3]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="70" sdnum="2052;">70</td>
    <td align="center">-</td>
    <td align="center" sdval="90" sdnum="2052;">90</td>
    <td align="center" sdval="84" sdnum="2052;">84</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
  </tr>
  <tr>
    <td height="20" align="center">Goel et al. [4] : wDTW</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="77.3" sdnum="2052;">77.3</td>
    <td align="center">-</td>
    <td align="center" sdval="89.7" sdnum="2052;">89.7</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">Un</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Bissacco et al. [5] : PhotoOCR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="90.4" sdnum="2052;">90.4</td>
    <td align="center" sdval="78" sdnum="2052;">78</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="87.6" sdnum="2052;">87.6</td>
    <td align="center">ExPr</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Phan et al. [6]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="73.7" sdnum="2052;">73.7</td>
    <td align="center">-</td>
    <td align="center" sdval="82.2" sdnum="2052;">82.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Alsharif et al. [7] : HMM/Maxout</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="74.3" sdnum="2052;">74.3</td>
    <td align="center">-</td>
    <td align="center" sdval="93.1" sdnum="2052;">93.1</td>
    <td align="center" sdval="88.6" sdnum="2052;">88.6</td>
    <td align="center" sdval="85.1" sdnum="2052;">85.1</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Almazan et al [8] : KCSR</td>
    <td align="center" sdval="88.6" sdnum="2052;">88.6</td>
    <td align="center" sdval="75.6" sdnum="2052;">75.6</td>
    <td align="center">-</td>
    <td align="center" sdval="87" sdnum="2052;">87</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Yao et al. [9] : Strokelets</td>
    <td align="center" sdval="80.2" sdnum="2052;">80.2</td>
    <td align="center" sdval="69.3" sdnum="2052;">69.3</td>
    <td align="center">-</td>
    <td align="center" sdval="75.9" sdnum="2052;">75.9</td>
    <td align="center">-</td>
    <td align="center" sdval="88.5" sdnum="2052;">88.5</td>
    <td align="center" sdval="80.3" sdnum="2052;">80.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">R.-Serrano et al.[10] : Label embedding</td>
    <td align="center" sdval="76.1" sdnum="2052;">76.1</td>
    <td align="center" sdval="57.4" sdnum="2052;">57.4</td>
    <td align="center">-</td>
    <td align="center" sdval="70" sdnum="2052;">70</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [11]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="86.1" sdnum="2052;">86.1</td>
    <td align="center">-</td>
    <td align="center" sdval="96.2" sdnum="2052;">96.2</td>
    <td align="center" sdval="91.5" sdnum="2052;">91.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Su and Lu [12]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="83" sdnum="2052;">83</td>
    <td align="center">-</td>
    <td align="center" sdval="92" sdnum="2052;">92</td>
    <td align="center" sdval="82" sdnum="2052;">82</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ACCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Gordo[13] : Mid-features</td>
    <td align="center" sdval="93.3" sdnum="2052;">93.3</td>
    <td align="center" sdval="86.6" sdnum="2052;">86.6</td>
    <td align="center">-</td>
    <td align="center" sdval="91.8" sdnum="2052;">91.8</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [14]</td>
    <td align="center" sdval="97.1" sdnum="2052;">97.1</td>
    <td align="center" sdval="92.7" sdnum="2052;">92.7</td>
    <td align="center">-</td>
    <td align="center" sdval="95.4" sdnum="2052;">95.4</td>
    <td align="center" sdval="80.7" sdnum="2052;">80.7</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="98.6" sdnum="2052;">98.6</td>
    <td align="center" sdval="93.3" sdnum="2052;">93.3</td>
    <td align="center" sdval="93.1" sdnum="2052;">93.1</td>
    <td align="center" sdval="90.8" sdnum="2052;">90.8</td>
    <td align="center">ExPr</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [15]</td>
    <td align="center" sdval="95.5" sdnum="2052;">95.5</td>
    <td align="center" sdval="89.6" sdnum="2052;">89.6</td>
    <td align="center">-</td>
    <td align="center" sdval="93.2" sdnum="2052;">93.2</td>
    <td align="center" sdval="71.7" sdnum="2052;">71.7</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center" sdval="97" sdnum="2052;">97</td>
    <td align="center" sdval="93.4" sdnum="2052;">93.4</td>
    <td align="center" sdval="89.6" sdnum="2052;">89.6</td>
    <td align="center" sdval="81.8" sdnum="2052;">81.8</td>
    <td align="center">SK + ExPr</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi, Bai, and Yao [16] : CRNN</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="81.2" sdnum="2052;">81.2</td>
    <td align="center" sdval="97.5" sdnum="2052;">97.5</td>
    <td align="center" sdval="82.7" sdnum="2052;">82.7</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center" sdval="95.7" sdnum="2052;"><b>95.7</b></td>
    <td align="center" sdval="91.9" sdnum="2052;">91.9</td>
    <td align="center" sdval="89.6" sdnum="2052;">89.6</td>
    <td align="center">SK</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [17] : RARE</td>
    <td align="center" sdval="96.2" sdnum="2052;">96.2</td>
    <td align="center" sdval="93.8" sdnum="2052;">93.8</td>
    <td align="center" sdval="81.9" sdnum="2052;">81.9</td>
    <td align="center" sdval="95.5" sdnum="2052;">95.5</td>
    <td align="center" sdval="81.9" sdnum="2052;">81.9</td>
    <td align="center" sdval="98.3" sdnum="2052;">98.3</td>
    <td align="center" sdval="96.2" sdnum="2052;">96.2</td>
    <td align="center" sdval="94.8" sdnum="2052;">94.8</td>
    <td align="center" sdval="90.1" sdnum="2052;">90.1</td>
    <td align="center" sdval="88.6" sdnum="2052;">88.6</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">Lee and Osindero [18] : R2AM</td>
    <td align="center" sdval="96.8" sdnum="2052;">96.8</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center" sdval="78.4" sdnum="2052;">78.4</td>
    <td align="center" sdval="96.3" sdnum="2052;">96.3</td>
    <td align="center" sdval="80.7" sdnum="2052;">80.7</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="97" sdnum="2052;">97</td>
    <td align="center">-</td>
    <td align="center" sdval="88.7" sdnum="2052;">88.7</td>
    <td align="center" sdval="90" sdnum="2052;">90</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [19] : STAR-Net</td>
    <td align="center" sdval="97.7" sdnum="2052;">97.7</td>
    <td align="center" sdval="94.5" sdnum="2052;">94.5</td>
    <td align="center" sdval="83.3" sdnum="2052;">83.3</td>
    <td align="center" sdval="95.5" sdnum="2052;">95.5</td>
    <td align="center" sdval="83.6" sdnum="2052;">83.6</td>
    <td align="center" sdval="96.9" sdnum="2052;">96.9</td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center">-</td>
    <td align="center" sdval="89.9" sdnum="2052;">89.9</td>
    <td align="center" sdval="89.1" sdnum="2052;">89.1</td>
    <td align="center">SK + ExPr</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liu et al. [78]</td>
    <td align="center" sdval="94.1" sdnum="2052;">94.1</td>
    <td align="center" sdval="84.7" sdnum="2052;">84.7</td>
    <td align="center">-</td>
    <td align="center" sdval="92.5" sdnum="2052;">92.5</td>
    <td align="center">-</td>
    <td align="center" sdval="96.8" sdnum="2052;">96.8</td>
    <td align="center" sdval="92.2" sdnum="2052;">92.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu (D_A)</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Mishra et al. [77]</td>
    <td align="center" sdval="78.07" sdnum="2052;">78.07</td>
    <td align="center">-</td>
    <td align="center" sdval="46.73" sdnum="2052;">46.73</td>
    <td align="center" sdval="78.2" sdnum="2052;">78.2</td>
    <td align="center">-</td>
    <td align="center" sdval="88" sdnum="2052;">88</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="67.7" sdnum="2052;">67.7</td>
    <td align="center" sdval="60.18" sdnum="2052;">60.18</td>
    <td align="center">ExPu (D_A)</td>
    <td align="center">CVIU</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Su and Lu [76]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="91" sdnum="2052;">91</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="89" sdnum="2052;">89</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="76" sdnum="2052;">76</td>
    <td align="center">SK + ExPu</td>
    <td align="center">PR</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yang et al. [20]</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center" sdval="96.1" sdnum="2052;">96.1</td>
    <td align="center">-</td>
    <td align="center" sdval="95.2" sdnum="2052;">95.2</td>
    <td align="center">-</td>
    <td align="center" sdval="97.7" sdnum="2052;">97.7</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">IJCAI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Yin et al. [21]</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="96.1" sdnum="2052;">96.1</td>
    <td align="center" sdval="78.2" sdnum="2052;">78.2</td>
    <td align="center" sdval="95.1" sdnum="2052;">95.1</td>
    <td align="center" sdval="72.5" sdnum="2052;">72.5</td>
    <td align="center" sdval="97.6" sdnum="2052;">97.6</td>
    <td align="center" sdval="96.5" sdnum="2052;">96.5</td>
    <td align="center">-</td>
    <td align="center" sdval="81.1" sdnum="2052;">81.1</td>
    <td align="center" sdval="81.4" sdnum="2052;">81.4</td>
    <td align="center">SK</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[66] : GRCNN</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center" sdval="95.6" sdnum="2052;">95.6</td>
    <td align="center" sdval="80.8" sdnum="2052;">80.8</td>
    <td align="center" sdval="96.3" sdnum="2052;">96.3</td>
    <td align="center" sdval="81.5" sdnum="2052;">81.5</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center">-</td>
    <td align="center" sdval="91.2" sdnum="2052;">91.2</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">*Cheng et al. [22] : FAN</td>
    <td align="center" sdval="99.3" sdnum="2052;">99.3</td>
    <td align="center" sdval="97.5" sdnum="2052;">97.5</td>
    <td align="center" sdval="87.4" sdnum="2052;">87.4</td>
    <td align="center" sdval="97.1" sdnum="2052;">97.1</td>
    <td align="center" sdval="85.9" sdnum="2052;">85.9</td>
    <td align="center" sdval="99.2" sdnum="2052;">99.2</td>
    <td align="center" sdval="97.3" sdnum="2052;">97.3</td>
    <td align="center">-</td>
    <td align="center" sdval="94.2" sdnum="2052;">94.2</td>
    <td align="center" sdval="93.3" sdnum="2052;">93.3</td>
    <td align="center">SK + ST (Pixel_wise)</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Cheng et al. [23] : AON</td>
    <td align="center" sdval="99.6" sdnum="2052;"><b>99.6</b></td>
    <td align="center" sdval="98.1" sdnum="2052;">98.1</td>
    <td align="center" sdval="87" sdnum="2052;">87</td>
    <td align="center" sdval="96" sdnum="2052;">96</td>
    <td align="center" sdval="82.8" sdnum="2052;">82.8</td>
    <td align="center" sdval="98.5" sdnum="2052;">98.5</td>
    <td align="center" sdval="97.1" sdnum="2052;">97.1</td>
    <td align="center">-</td>
    <td align="center" sdval="91.5" sdnum="2052;">91.5</td>
    <td align="center">-</td>
    <td align="center">SK + ST (D_A)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [24]</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="81.8" sdnum="2052;">81.8</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="82.7" sdnum="2052;">82.7</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="96.7" sdnum="2052;">96.7</td>
    <td align="center">-</td>
    <td align="center" sdval="89.2" sdnum="2052;">89.2</td>
    <td align="center" sdval="88" sdnum="2052;">88</td>
    <td align="center">SK</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [25] : Char-Net</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="83.6" sdnum="2052;">83.6</td>
    <td align="center">-</td>
    <td align="center" sdval="84.4" sdnum="2052;">84.4</td>
    <td align="center">-</td>
    <td align="center" sdval="93.3" sdnum="2052;">93.3</td>
    <td align="center">-</td>
    <td align="center" sdval="91.5" sdnum="2052;">91.5</td>
    <td align="center" sdval="90.8" sdnum="2052;">90.8</td>
    <td align="center">SK (D_A)</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liu et al.  [26] : SqueezedText</td>
    <td align="center" sdval="97" sdnum="2052;">97</td>
    <td align="center" sdval="94.1" sdnum="2052;">94.1</td>
    <td align="center" sdval="87" sdnum="2052;">87</td>
    <td align="center" sdval="95.2" sdnum="2052;">95.2</td>
    <td align="center">-</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="93.8" sdnum="2052;">93.8</td>
    <td align="center" sdval="93.1" sdnum="2052;">93.1</td>
    <td align="center" sdval="92.9" sdnum="2052;">92.9</td>
    <td align="center">ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhan et al.[73]</td>
    <td align="center" sdval="98.1" sdnum="2052;">98.1</td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center" sdval="79.3" sdnum="2052;">79.3</td>
    <td align="center" sdval="96.7" sdnum="2052;">96.7</td>
    <td align="center" sdval="81.5" sdnum="2052;">81.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="87.1" sdnum="2052;">87.1</td>
    <td align="center">Pr(5 million)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Bai et al. [27] : EP</td>
    <td align="center" sdval="99.5" sdnum="2052;">99.5</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="88.3" sdnum="2052;">88.3</td>
    <td align="center" sdval="96.6" sdnum="2052;">96.6</td>
    <td align="center" sdval="87.5" sdnum="2052;">87.5</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center">-</td>
    <td align="center" sdval="94.6" sdnum="2052;">94.6</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center">SK + ST (Pixel_wise)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Fang et al.[74]</td>
    <td align="center" sdval="98.5" sdnum="2052;">98.5</td>
    <td align="center" sdval="96.8" sdnum="2052;">96.8</td>
    <td align="center" sdval="86.7" sdnum="2052;">86.7</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center" sdval="86.7" sdnum="2052;">86.7</td>
    <td align="center" sdval="99.3" sdnum="2052;"><b>99.3</b></td>
    <td align="center" sdval="98.4" sdnum="2052;">98.4</td>
    <td align="center">-</td>
    <td align="center" sdval="94.8" sdnum="2052;">94.8</td>
    <td align="center" sdval="93.5" sdnum="2052;">93.5</td>
    <td align="center">SK + ST</td>
    <td align="center">MultiMedia</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.[75] : EnEsCTC</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="82" sdnum="2052;">82</td>
    <td align="center">-</td>
    <td align="center" sdval="80.6" sdnum="2052;">80.6</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="92" sdnum="2052;">92</td>
    <td align="center" sdval="90.6" sdnum="2052;">90.6</td>
    <td align="center">SK</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al. [28]</td>
    <td align="center" sdval="97.3" sdnum="2052;">97.3</td>
    <td align="center" sdval="96.1" sdnum="2052;">96.1</td>
    <td align="center" sdval="89.4" sdnum="2052;">89.4</td>
    <td align="center" sdval="96.8" sdnum="2052;">96.8</td>
    <td align="center" sdval="87.1" sdnum="2052;">87.1</td>
    <td align="center" sdval="98.1" sdnum="2052;">98.1</td>
    <td align="center" sdval="97.5" sdnum="2052;">97.5</td>
    <td align="center">-</td>
    <td align="center" sdval="94.7" sdnum="2052;">94.7</td>
    <td align="center" sdval="94" sdnum="2052;">94</td>
    <td align="center">SK</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[61] : MAAN</td>
    <td align="center" sdval="98.3" sdnum="2052;">98.3</td>
    <td align="center" sdval="96.4" sdnum="2052;">96.4</td>
    <td align="center" sdval="84.1" sdnum="2052;">84.1</td>
    <td align="center" sdval="96.4" sdnum="2052;">96.4</td>
    <td align="center" sdval="83.5" sdnum="2052;">83.5</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="96.4" sdnum="2052;">96.4</td>
    <td align="center">-</td>
    <td align="center" sdval="92.2" sdnum="2052;">92.2</td>
    <td align="center" sdval="91.1" sdnum="2052;">91.1</td>
    <td align="center">SK</td>
    <td align="center">ICFHR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [29]</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="97.2" sdnum="2052;">97.2</td>
    <td align="center" sdval="83.6" sdnum="2052;">83.6</td>
    <td align="center" sdval="97.7" sdnum="2052;">97.7</td>
    <td align="center" sdval="83.9" sdnum="2052;">83.9</td>
    <td align="center" sdval="98.6" sdnum="2052;">98.6</td>
    <td align="center" sdval="96.6" sdnum="2052;">96.6</td>
    <td align="center">-</td>
    <td align="center" sdval="91.4" sdnum="2052;">91.4</td>
    <td align="center" sdval="89.5" sdnum="2052;">89.5</td>
    <td align="center">SK</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [30] : ASTER</td>
    <td align="center" sdval="99.6" sdnum="2052;"><b>99.6</b></td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="93.4" sdnum="2052;">93.4</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="89.5" sdnum="2052;">89.5</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center">-</td>
    <td align="center" sdval="94.5" sdnum="2052;">94.5</td>
    <td align="center" sdval="91.8" sdnum="2052;">91.8</td>
    <td align="center">SK + ST</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : ASTER + AEG</td>
    <td align="center" sdval="99.5" sdnum="2052;">99.5</td>
    <td align="center" sdval="98.5" sdnum="2052;">98.5</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="90.3" sdnum="2052;">90.3</td>
    <td align="center" sdval="99" sdnum="2052;">99</td>
    <td align="center" sdval="98.3" sdnum="2052;">98.3</td>
    <td align="center">-</td>
    <td align="center" sdval="95.2" sdnum="2052;">95.2</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [46] : MORAN</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="96.2" sdnum="2052;">96.2</td>
    <td align="center" sdval="91.2" sdnum="2052;">91.2</td>
    <td align="center" sdval="96.6" sdnum="2052;">96.6</td>
    <td align="center" sdval="88.3" sdnum="2052;">88.3</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="92.4" sdnum="2052;">92.4</td>
    <td align="center">SK + ST</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [61] : MORAN-v2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="93.4" sdnum="2052;">93.4</td>
    <td align="center">-</td>
    <td align="center" sdval="88.3" sdnum="2052;">88.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.2" sdnum="2052;">94.2</td>
    <td align="center" sdval="93.2" sdnum="2052;">93.2</td>
    <td align="center">SK + ST</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : MORAN-v2 + AEG</td>
    <td align="center" sdval="99.5" sdnum="2052;">99.5</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="94.6" sdnum="2052;">94.6</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="90.4" sdnum="2052;">90.4</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="98.3" sdnum="2052;">98.3</td>
    <td align="center">-</td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Xie et al. [47] : CAN</td>
    <td align="center" sdval="97" sdnum="2052;">97</td>
    <td align="center" sdval="94.2" sdnum="2052;">94.2</td>
    <td align="center" sdval="80.5" sdnum="2052;">80.5</td>
    <td align="center" sdval="96.9" sdnum="2052;">96.9</td>
    <td align="center" sdval="83.4" sdnum="2052;">83.4</td>
    <td align="center" sdval="98.4" sdnum="2052;">98.4</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center">-</td>
    <td align="center" sdval="91" sdnum="2052;">91</td>
    <td align="center" sdval="90.5" sdnum="2052;">90.5</td>
    <td align="center">SK</td>
    <td align="center">ACM</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liao et al.[48] : CA-FCN</td>
    <td align="center"><b>^99.8</b></td>
    <td align="center" sdval="98.9" sdnum="2052;">98.9</td>
    <td align="center" sdval="92" sdnum="2052;">92</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="82.1" sdnum="2052;">82.1</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="91.4" sdnum="2052;">91.4</td>
    <td align="center">SK + ST+ ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Li et al. [49] : SAR</td>
    <td align="center" sdval="99.4" sdnum="2052;">99.4</td>
    <td align="center" sdval="98.2" sdnum="2052;">98.2</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="98.5" sdnum="2052;">98.5</td>
    <td align="center" sdval="91.2" sdnum="2052;">91.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94" sdnum="2052;">94</td>
    <td align="center">SK + ST + ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="23" align="center">Zhan el at. [55]: ESIR</td>
    <td align="center" sdval="99.6" sdnum="2052;"><b>99.6</b></td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="93.3" sdnum="2052;">93.3</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="90.2" sdnum="2052;">90.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="91.3" sdnum="2052;">91.3</td>
    <td align="center">SK + ST</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [56]: SSDAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="83.8" sdnum="2052;">83.8</td>
    <td align="center">-</td>
    <td align="center" sdval="84.5" sdnum="2052;">84.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="92.1" sdnum="2052;">92.1</td>
    <td align="center" sdval="91.8" sdnum="2052;">91.8</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yang et al. [62]: ScRN</td>
    <td align="center" sdval="99.5" sdnum="2052;">99.5</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center" sdval="97.2" sdnum="2052;">97.2</td>
    <td align="center" sdval="88.9" sdnum="2052;">88.9</td>
    <td align="center" sdval="99" sdnum="2052;">99</td>
    <td align="center" sdval="98.3" sdnum="2052;">98.3</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="93.9" sdnum="2052;">93.9</td>
    <td align="center">SK + ST(char-level + word-level)</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [64]: GCAM</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="93.9" sdnum="2052;">93.9</td>
    <td align="center">-</td>
    <td align="center" sdval="91.3" sdnum="2052;">91.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center" sdval="95.7" sdnum="2052;">95.7</td>
    <td align="center">SK + ST</td>
    <td align="center">ICME</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Jeonghun et al. [65]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="87.9" sdnum="2052;">87.9</td>
    <td align="center">-</td>
    <td align="center" sdval="87.5" sdnum="2052;">87.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center" sdval="92.3" sdnum="2052;">92.3</td>
    <td align="center">SK + ST</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="26" align="center">Huang et al. [67]：EPAN</td>
    <td align="center" sdval="98.9" sdnum="2052;">98.9</td>
    <td align="center" sdval="97.8" sdnum="2052;">97.8</td>
    <td align="center" sdval="94" sdnum="2052;">94</td>
    <td align="center" sdval="96.6" sdnum="2052;">96.6</td>
    <td align="center" sdval="88.9" sdnum="2052;">88.9</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="94.5" sdnum="2052;">94.5</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [68]</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center" sdval="81.8" sdnum="2052;">81.8</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="82.7" sdnum="2052;">82.7</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center" sdval="96.7" sdnum="2052;">96.7</td>
    <td align="center">-</td>
    <td align="center" sdval="89.2" sdnum="2052;">89.2</td>
    <td align="center" sdval="88" sdnum="2052;">88</td>
    <td align="center">SK</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Qi et al. [69] : CCL</td>
    <td align="center" sdval="99.6" sdnum="2052;">99.6</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="91.1" sdnum="2052;">91.1</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center" sdval="85.9" sdnum="2052;">85.9</td>
    <td align="center" sdval="99.2" sdnum="2052;">99.2</td>
    <td align="center"><b>^98.8</b></td>
    <td align="center">-</td>
    <td align="center" sdval="93.5" sdnum="2052;">93.5</td>
    <td align="center" sdval="92.8" sdnum="2052;">92.8</td>
    <td align="center">SK + ST(char-level + word-level)</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Wang et al. [70] : ReELFA</td>
    <td align="center" sdval="99.2" sdnum="2052;">99.2</td>
    <td align="center" sdval="98.1" sdnum="2052;">98.1</td>
    <td align="center" sdval="90.9" sdnum="2052;">90.9</td>
    <td align="center">-</td>
    <td align="center" sdval="82.7" sdnum="2052;">82.7</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ST(char-level + word-level)</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhu et al. [71] : HATN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="88.6" sdnum="2052;">88.6</td>
    <td align="center">-</td>
    <td align="center" sdval="82.2" sdnum="2052;">82.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="91.3" sdnum="2052;">91.3</td>
    <td align="center" sdval="91.1" sdnum="2052;">91.1</td>
    <td align="center">SK(D_A) + Pu</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhan et al. [72] : SF-GAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="63" sdnum="2052;">63</td>
    <td align="center">-</td>
    <td align="center" sdval="69.3" sdnum="2052;">69.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="61.8" sdnum="2052;">61.8</td>
    <td align="center">Pr(1 million)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Liao et al. [79] : SAM</td>
    <td align="center" sdval="99.4" sdnum="2052;">99.4</td>
    <td align="center" sdval="98.6" sdnum="2052;">98.6</td>
    <td align="center" sdval="93.9" sdnum="2052;">93.9</td>
    <td align="center" sdval="98.6" sdnum="2052;">98.6</td>
    <td align="center" sdval="90.6" sdnum="2052;">90.6</td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center">-</td>
    <td align="center" sdval="95.2" sdnum="2052;">95.2</td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center">SK + ST</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liao et al. [79] : seg-SAM</td>
    <td align="center"><b>^99.8</b></td>
    <td align="center"><b>^99.3</b></td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="91.8" sdnum="2052;">91.8</td>
    <td align="center" sdval="99" sdnum="2052;">99</td>
    <td align="center" sdval="97.9" sdnum="2052;">97.9</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="95.3" sdnum="2052;">95.3</td>
    <td align="center">SK + ST (char-level)</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [80] : DAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.3" sdnum="2052;">94.3</td>
    <td align="center">-</td>
    <td align="center" sdval="89.2" sdnum="2052;">89.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center" sdval="93.9" sdnum="2052;">93.9</td>
    <td align="center">SK + ST</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [82] : TextSR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="92.5" sdnum="2052;">92.5</td>
    <td align="center" sdval="98" sdnum="2052;">98</td>
    <td align="center" sdval="87.2" sdnum="2052;">87.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="93.2" sdnum="2052;">93.2</td>
    <td align="center" sdval="91.3" sdnum="2052;">91.3</td>
    <td align="center">SK + ST</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Wan et al. [83] : TextScanner</td>
    <td align="center" sdval="99.7" sdnum="2052;">99.7</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="93.9" sdnum="2052;">93.9</td>
    <td align="center" sdval="98.5" sdnum="2052;">98.5</td>
    <td align="center" sdval="90.1" sdnum="2052;">90.1</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="92.9" sdnum="2052;">92.9</td>
    <td align="center">SK + ST (char-level)</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">*Hu et al. [84] : GTC</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"><b>^95.8</b></td>
    <td align="center">-</td>
    <td align="center"><b>^92.9</b></td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="95.5" sdnum="2052;">95.5</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center">SK + ST + ExPu</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [85]</td>
    <td align="center" sdval="99.6" sdnum="2052;"><b>99.6</b></td>
    <td align="center" sdval="98.8" sdnum="2052;">98.8</td>
    <td align="center" sdval="95.6" sdnum="2052;"><b>95.6</b></td>
    <td align="center" sdval="99.4" sdnum="2052;"><b>99.4</b></td>
    <td align="center" sdval="92.9" sdnum="2052;"><b>92.9</b></td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="98.8" sdnum="2052;"><b>98.8</b></td>
    <td align="center">-</td>
    <td align="center" sdval="96.2" sdnum="2052;"><b>96.2</b></td>
    <td align="center" sdval="96" sdnum="2052;"><b>96</b></td>
    <td align="center">SK + ST</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">*Litman et al. [86]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="93.7" sdnum="2052;">93.7</td>
    <td align="center">-</td>
    <td align="center" sdval="92.7" sdnum="2052;">92.7</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"><b>^96.3</b></td>
    <td align="center" sdval="93.9" sdnum="2052;">93.9</td>
    <td align="center">SK + ST + ExPu </td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Yu et al. [87]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.8" sdnum="2052;">94.8</td>
    <td align="center">-</td>
    <td align="center" sdval="91.5" sdnum="2052;">91.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="95.5" sdnum="2052;">95.5</td>
    <td align="center">SK + ST</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Qiao et al. [101] : SEED</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="93.8" sdnum="2052;">93.8</td>
    <td align="center">-</td>
    <td align="center" sdval="89.6" sdnum="2052;">89.6</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="92.8" sdnum="2052;">92.8</td>
    <td align="center">SK + ST</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Bleeker et al. [93] : Bi-STET</td>
    <td align="center" sdval="99.6" sdnum="2052;"><b>99.6</b></td>
    <td align="center" sdval="98.9" sdnum="2052;"><b>98.9</b></td>
    <td align="center" sdval="94.7" sdnum="2052;">94.7</td>
    <td align="center" sdval="97.4" sdnum="2052;">97.4</td>
    <td align="center" sdval="89" sdnum="2052;">89</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="98.7" sdnum="2052;">98.7</td>
    <td align="center">-</td>
    <td align="center" sdval="96" sdnum="2052;">96</td>
    <td align="center" sdval="93.4" sdnum="2052;">93.4</td>
    <td align="center">SK + ST</td>
    <td align="center">ECAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">*Bartz et al. [94] : KISS</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.6" sdnum="2052;">94.6</td>
    <td align="center">-</td>
    <td align="center" sdval="89.2" sdnum="2052;">89.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="93.1" sdnum="2052;">93.1</td>
    <td align="center">SK + ST + ExPu (D_A)</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [95] : SPIN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.7" sdnum="2052;">94.7</td>
    <td align="center">-</td>
    <td align="center" sdval="90.3" sdnum="2052;">90.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center" sdval="92.8" sdnum="2052;">92.8</td>
    <td align="center">SK + ST</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Lin et al. [96] : FASDA</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="96.5" sdnum="2052;">96.5</td>
    <td align="center" sdval="88.3" sdnum="2052;">88.3</td>
    <td align="center" sdval="99.1" sdnum="2052;">99.1</td>
    <td align="center" sdval="97.5" sdnum="2052;">97.5</td>
    <td align="center">-</td>
    <td align="center" sdval="94.8" sdnum="2052;">94.8</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center">SK</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [98] : AutoSTR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.7" sdnum="2052;">94.7</td>
    <td align="center">-</td>
    <td align="center" sdval="90.9" sdnum="2052;">90.9</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="93.3" sdnum="2052;">93.3</td>
    <td align="center" sdval="94.2" sdnum="2052;">94.2</td>
    <td align="center">SK + ST</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Mou et al. [99] : PlugNet</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center">-</td>
    <td align="center" sdval="92.3" sdnum="2052;">92.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="95.7" sdnum="2052;">95.7</td>
    <td align="center" sdval="95" sdnum="2052;">95</td>
    <td align="center">SK + ST</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yue et al. [100] : RobustScanner</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="95.4" sdnum="2052;">95.4</td>
    <td align="center">-</td>
    <td align="center" sdval="89.3" sdnum="2052;">89.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="94.1" sdnum="2052;">94.1</td>
    <td align="center">SK + ST + ExPu</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
</table>
<a id="222-performance-comparison-of-recognition-algorithms-on-irregular-latin-datasets"></a>

#### 2.2.2 Performance Comparison of Recognition Algorithms on Irregular Latin Datasets

<table cellspacing="0" border="0">
  <colgroup width="271"></colgroup>
  <colgroup span="6" width="86"></colgroup>
  <colgroup width="103"></colgroup>
  <colgroup width="172"></colgroup>
  <colgroup span="2" width="86"></colgroup>
  <tr>
    <td colspan=11 height="34" align="center"><b>Performance Comparison of Recognition Algorithms on Irregular Latin Datasets</b></td>
    </tr>
  <tr>
    <td rowspan=2 height="39" align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Method&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td colspan=3 align="center">SVT-P</td>
    <td align="center">CUTE80</td>
    <td align="center">IC15-S</td>
    <td align="center">IC15</td>
    <td align="center">COCO-TEXT</td>
    <td rowspan=2 align="center">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Data&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td rowspan=2 align="center">Source</td>
    <td rowspan=2 align="center">Time</td>
  </tr>
  <tr>
    <td align="center" sdval="50" sdnum="2052;">50</td>
    <td align="center">Full</td>
    <td align="center">None</td>
    <td align="center">None</td>
    <td align="center">None</td>
    <td align="center">None</td>
    <td align="center">None</td>
    </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : ABBYY</td>
    <td align="center" sdval="40.5" sdnum="2052;">40.5</td>
    <td align="center" sdval="26.1" sdnum="2052;">26.1</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">Un</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [1] : SYNTH+PLEX</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2011" sdnum="2052;">2011</td>
  </tr>
  <tr>
    <td height="20" align="center">Mishra et al. [2]</td>
    <td align="center" sdval="45.7" sdnum="2052;">45.7</td>
    <td align="center" sdval="24.7" sdnum="2052;">24.7</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [3]</td>
    <td align="center" sdval="40.2" sdnum="2052;">40.2</td>
    <td align="center" sdval="32.4" sdnum="2052;">32.4</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2012" sdnum="2052;">2012</td>
  </tr>
  <tr>
    <td height="20" align="center">Goel et al. [4] : wDTW</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">Un</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Bissacco et al. [5] : PhotoOCR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Phan et al. [6]</td>
    <td align="center" sdval="62.3" sdnum="2052;">62.3</td>
    <td align="center" sdval="42.2" sdnum="2052;">42.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2013" sdnum="2052;">2013</td>
  </tr>
  <tr>
    <td height="20" align="center">Alsharif et al. [7] : HMM/Maxout</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Almazan et al [8] : KCSR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Yao et al. [9] : Strokelets</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">R.-Serrano et al.[10] : Label embedding</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [11]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Su and Lu [12]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">ACCV</td>
    <td align="center" sdval="2014" sdnum="2052;">2014</td>
  </tr>
  <tr>
    <td height="20" align="center">Gordo[13] : Mid-features</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [14]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Jaderberg et al. [15]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ExPr</td>
    <td align="center">ICLR</td>
    <td align="center" sdval="2015" sdnum="2052;">2015</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi, Bai, and Yao [16] : CRNN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [17] : RARE</td>
    <td align="center" sdval="91.2" sdnum="2052;">91.2</td>
    <td align="center" sdval="77.4" sdnum="2052;">77.4</td>
    <td align="center" sdval="71.8" sdnum="2052;">71.8</td>
    <td align="center" sdval="59.2" sdnum="2052;">59.2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">Lee and Osindero [18] : R2AM</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [19] : STAR-Net</td>
    <td align="center" sdval="94.3" sdnum="2052;">94.3</td>
    <td align="center" sdval="83.6" sdnum="2052;">83.6</td>
    <td align="center" sdval="73.5" sdnum="2052;">73.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ExPr</td>
    <td align="center">BMVC</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liu et al. [78]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu (D_A)</td>
    <td align="center">ICPR</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Mishra et al. [77]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu (D_A)</td>
    <td align="center">CVIU</td>
    <td align="center" sdval="2016" sdnum="2052;">2016</td>
  </tr>
  <tr>
    <td height="20" align="center">*Su and Lu [76]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ExPu</td>
    <td align="center">PR</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yang et al. [20]</td>
    <td align="center" sdval="93" sdnum="2052;">93</td>
    <td align="center" sdval="80.2" sdnum="2052;">80.2</td>
    <td align="center" sdval="75.8" sdnum="2052;">75.8</td>
    <td align="center" sdval="69.3" sdnum="2052;">69.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPu</td>
    <td align="center">IJCAI</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Yin et al. [21]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[66] : GRCNN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">*Cheng et al. [22] : FAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="70.6" sdnum="2052;">70.6</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ST (Pixel_wise)</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2017" sdnum="2052;">2017</td>
  </tr>
  <tr>
    <td height="20" align="center">Cheng et al. [23] : AON</td>
    <td align="center" sdval="94" sdnum="2052;">94</td>
    <td align="center" sdval="83.7" sdnum="2052;">83.7</td>
    <td align="center" sdval="73" sdnum="2052;">73</td>
    <td align="center" sdval="76.8" sdnum="2052;">76.8</td>
    <td align="center">-</td>
    <td align="center" sdval="68.2" sdnum="2052;">68.2</td>
    <td align="center">-</td>
    <td align="center">SK + ST (D_A)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [24]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.  [25] : Char-Net</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="73.5" sdnum="2052;">73.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="60" sdnum="2052;">60</td>
    <td align="center">-</td>
    <td align="center">SK (D_A)</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liu et al.  [26] : SqueezedText</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhan et al.[73]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">Pr(5 million)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">*Bai et al. [27] : EP</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="73.9" sdnum="2052;">73.9</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ST (Pixel_wise)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Fang et al.[74]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="71.2" sdnum="2052;">71.2</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">MultiMedia</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al.[75] : EnEsCTC</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">NIPS</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Liu et al. [28]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="73.9" sdnum="2052;">73.9</td>
    <td align="center" sdval="62.5" sdnum="2052;">62.5</td>
    <td align="center"><br></td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al.[61] : MAAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">ICFHR</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [29]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Shi et al. [30] : ASTER</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="78.5" sdnum="2052;">78.5</td>
    <td align="center" sdval="79.5" sdnum="2052;">79.5</td>
    <td align="center" sdval="76.1" sdnum="2052;">76.1</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2018" sdnum="2052;">2018</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : ASTER + AEG</td>
    <td align="center" sdval="94.4" sdnum="2052;">94.4</td>
    <td align="center" sdval="89.5" sdnum="2052;">89.5</td>
    <td align="center" sdval="82" sdnum="2052;">82</td>
    <td align="center" sdval="80.9" sdnum="2052;">80.9</td>
    <td align="center">-</td>
    <td align="center" sdval="76.7" sdnum="2052;">76.7</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [46] : MORAN</td>
    <td align="center" sdval="94.3" sdnum="2052;">94.3</td>
    <td align="center" sdval="86.7" sdnum="2052;">86.7</td>
    <td align="center" sdval="76.1" sdnum="2052;">76.1</td>
    <td align="center" sdval="77.4" sdnum="2052;">77.4</td>
    <td align="center">-</td>
    <td align="center" sdval="68.8" sdnum="2052;">68.8</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [61] : MORAN-v2</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="79.7" sdnum="2052;">79.7</td>
    <td align="center" sdval="81.9" sdnum="2052;">81.9</td>
    <td align="center">-</td>
    <td align="center" sdval="73.9" sdnum="2052;">73.9</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">PR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Chen et al. [60] : MORAN-v2 + AEG</td>
    <td align="center" sdval="94.7" sdnum="2052;">94.7</td>
    <td align="center" sdval="89.6" sdnum="2052;">89.6</td>
    <td align="center" sdval="82.8" sdnum="2052;">82.8</td>
    <td align="center" sdval="81.3" sdnum="2052;">81.3</td>
    <td align="center">-</td>
    <td align="center" sdval="77.4" sdnum="2052;">77.4</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Xie et al. [47] : CAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">ACM</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liao et al.[48] : CA-FCN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="78.1" sdnum="2052;">78.1</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ST+ ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Li et al. [49] : SAR</td>
    <td align="center"><b>^95.8</b></td>
    <td align="center" sdval="91.2" sdnum="2052;">91.2</td>
    <td align="center">^86.4</td>
    <td align="center" sdval="89.6" sdnum="2052;">89.6</td>
    <td align="center">-</td>
    <td align="center" sdval="78.8" sdnum="2052;">78.8</td>
    <td align="center"><b>^66.8</b></td>
    <td align="center">SK + ST + ExPr</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="23" align="center">Zhan el at. [55]: ESIR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="79.6" sdnum="2052;">79.6</td>
    <td align="center" sdval="83.3" sdnum="2052;">83.3</td>
    <td align="center">-</td>
    <td align="center" sdval="76.9" sdnum="2052;">76.9</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [56]: SSDAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yang et al. [62]: ScRN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="80.8" sdnum="2052;">80.8</td>
    <td align="center" sdval="87.5" sdnum="2052;">87.5</td>
    <td align="center">-</td>
    <td align="center" sdval="78.7" sdnum="2052;">78.7</td>
    <td align="center">-</td>
    <td align="center">SK + ST(char-level + word-level)</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [64]: GCAM</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="85.7" sdnum="2052;"><b>85.7</b></td>
    <td align="center" sdval="83.3" sdnum="2052;">83.3</td>
    <td align="center" sdval="83.5" sdnum="2052;">83.5</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">ICME</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Jeonghun et al. [65]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="79.2" sdnum="2052;">79.2</td>
    <td align="center" sdval="74" sdnum="2052;">74</td>
    <td align="center">-</td>
    <td align="center" sdval="71.8" sdnum="2052;">71.8</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">ICCV</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="26" align="center">Huang et al. [67]：EPAN</td>
    <td align="center" sdval="91.2" sdnum="2052;">91.2</td>
    <td align="center" sdval="86.4" sdnum="2052;">86.4</td>
    <td align="center" sdval="79.4" sdnum="2052;">79.4</td>
    <td align="center" sdval="82.6" sdnum="2052;">82.6</td>
    <td align="center">-</td>
    <td align="center" sdval="73.9" sdnum="2052;">73.9</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Gao et al. [68]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="62.3" sdnum="2052;">62.3</td>
    <td align="center" sdval="40" sdnum="2052;">40</td>
    <td align="center">SK</td>
    <td align="center">NC</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Qi et al. [69] : CCL</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="72.9" sdnum="2052;">72.9</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ST(char-level + word-level)</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Wang et al. [70] : ReELFA</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="82.3" sdnum="2052;">82.3</td>
    <td align="center">-</td>
    <td align="center" sdval="68.5" sdnum="2052;">68.5</td>
    <td align="center">-</td>
    <td align="center">ST(char-level + word-level)</td>
    <td align="center">ICDAR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhu et al. [71] : HATN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="73.5" sdnum="2052;">73.5</td>
    <td align="center" sdval="75.7" sdnum="2052;">75.7</td>
    <td align="center">-</td>
    <td align="center" sdval="70.1" sdnum="2052;">70.1</td>
    <td align="center">-</td>
    <td align="center">SK(D_A) + Pu</td>
    <td align="center">ICIP</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Zhan et al. [72] : SF-GAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="48.6" sdnum="2052;">48.6</td>
    <td align="center" sdval="40.6" sdnum="2052;">40.6</td>
    <td align="center">-</td>
    <td align="center" sdval="39" sdnum="2052;">39</td>
    <td align="center">-</td>
    <td align="center">Pr(1 million)</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Liao et al. [79] : SAM</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="82.2" sdnum="2052;">82.2</td>
    <td align="center" sdval="87.8" sdnum="2052;">87.8</td>
    <td align="center">-</td>
    <td align="center" sdval="77.3" sdnum="2052;">77.3</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Liao et al. [79] : seg-SAM</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="83.6" sdnum="2052;">83.6</td>
    <td align="center" sdval="88.5" sdnum="2052;">88.5</td>
    <td align="center">-</td>
    <td align="center" sdval="78.2" sdnum="2052;">78.2</td>
    <td align="center">-</td>
    <td align="center">SK + ST (char-level)</td>
    <td align="center">TPAMI</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [80] : DAN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="80" sdnum="2052;">80</td>
    <td align="center" sdval="84.4" sdnum="2052;">84.4</td>
    <td align="center">-</td>
    <td align="center" sdval="74.5" sdnum="2052;">74.5</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Wang et al. [82] : TextSR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="77.4" sdnum="2052;">77.4</td>
    <td align="center" sdval="78.9" sdnum="2052;">78.9</td>
    <td align="center">-</td>
    <td align="center" sdval="75.6" sdnum="2052;">75.6</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2019" sdnum="2052;">2019</td>
  </tr>
  <tr>
    <td height="20" align="center">*Wan et al. [83] : TextScanner</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="84.3" sdnum="2052;">84.3</td>
    <td align="center" sdval="83.3" sdnum="2052;">83.3</td>
    <td align="center">-</td>
    <td align="center" sdval="79.4" sdnum="2052;">79.4</td>
    <td align="center">-</td>
    <td align="center">SK + ST (char-level)</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">*Hu et al. [84] : GTC</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="85.7" sdnum="2052;">85.7</td>
    <td align="center" sdval="92.2" sdnum="2052;">92.2</td>
    <td align="center">-</td>
    <td align="center" sdval="79.5" sdnum="2052;">79.5</td>
    <td align="center">-</td>
    <td align="center">SK + ST + ExPu</td>
    <td align="center">AAAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Luo et al. [85]</td>
    <td align="center" sdval="95.8" sdnum="2052;"><b>95.8</b></td>
    <td align="center" sdval="91.5" sdnum="2052;"><b>91.5</b></td>
    <td align="center" sdval="85.1" sdnum="2052;">85.1</td>
    <td align="center" sdval="91.3" sdnum="2052;"><b>91.3</b></td>
    <td align="center" sdval="83.9" sdnum="2052;"><b>83.9</b></td>
    <td align="center" sdval="81.4" sdnum="2052;"><b>81.4</b></td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">IJCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">*Litman et al. [86]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center"><b>^86.9</b></td>
    <td align="center" sdval="87.5" sdnum="2052;">87.5</td>
    <td align="center">-</td>
    <td align="center" sdval="82.2" sdnum="2052;">82.2</td>
    <td align="center">-</td>
    <td align="center">SK + ST + ExPu </td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Yu et al. [87]</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="85.1" sdnum="2052;">85.1</td>
    <td align="center" sdval="87.8" sdnum="2052;">87.8</td>
    <td align="center" sdval="82.7" sdnum="2052;">82.7</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Qiao et al. [101] : SEED</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="81.4" sdnum="2052;">81.4</td>
    <td align="center" sdval="83.6" sdnum="2052;">83.6</td>
    <td align="center" sdval="80" sdnum="2052;">80</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">CVPR</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Bleeker et al. [93] : Bi-STET</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="80.6" sdnum="2052;">80.6</td>
    <td align="center" sdval="82.5" sdnum="2052;">82.5</td>
    <td align="center" sdval="75.7" sdnum="2052;">75.7</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">ECAI</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">*Bartz et al. [94] : KISS</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="83.1" sdnum="2052;">83.1</td>
    <td align="center" sdval="89.6" sdnum="2052;">89.6</td>
    <td align="center" sdval="80.3" sdnum="2052;">80.3</td>
    <td align="center" sdval="74.2" sdnum="2052;">74.2</td>
    <td align="center">-</td>
    <td align="center">SK + ST + ExPu (D_A)</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [95] : SPIN</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="82.8" sdnum="2052;">82.8</td>
    <td align="center" sdval="87.5" sdnum="2052;">87.5</td>
    <td align="center" sdval="82.2" sdnum="2052;">82.2</td>
    <td align="center" sdval="78.5" sdnum="2052;">78.5</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Lin et al. [96] : FASDA</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="73.3" sdnum="2052;">73.3</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK</td>
    <td align="center">arXiv</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Zhang et al. [98] : AutoSTR</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="81.7" sdnum="2052;">81.7</td>
    <td align="center">-</td>
    <td align="center" sdval="81.8" sdnum="2052;">81.8</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">Mou et al. [99] : PlugNet</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="84.3" sdnum="2052;">84.3</td>
    <td align="center" sdval="85" sdnum="2052;">85</td>
    <td align="center">-</td>
    <td align="center" sdval="82.2" sdnum="2052;">82.2</td>
    <td align="center">-</td>
    <td align="center">SK + ST</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
  <tr>
    <td height="20" align="center">*Yue et al. [100] : RobustScanner</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center" sdval="82.9" sdnum="2052;">82.9</td>
    <td align="center"><b>^92.4</b></td>
    <td align="center">-</td>
    <td align="center" sdval="79.2" sdnum="2052;">79.2</td>
    <td align="center">-</td>
    <td align="center">SK + ST + ExPu</td>
    <td align="center">ECCV</td>
    <td align="center" sdval="2020" sdnum="2052;">2020</td>
  </tr>
</table>

***

<a id="3-survey"></a>
## 3. Survey

**[50] \[TPAMI-2015]** Q. Ye and D. Doermann, “Text detection and recognition in imagery: A survey,” IEEE Trans. Pattern Anal. Mach. Intell, vol. 37, no. 7, pp. 1480–1500, 2015. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6945320)

**[51] \[Frontiers-Comput. Sci-2016]** Y. Zhu, C. Yao, and X. Bai, “Scene text detection and recognition: Recent advances and future trends,” Frontiers of Computer Science, vol. 10, no. 1, pp. 19–36, 2016. [paper](https://link.springer.com/article/10.1007/s11704-015-4488-0)

**[52] \[IJCV-2020]**  Long S, He X, Yao C. Scene text detection and recognition: The deep learning era[J]. International Journal of Computer Vision, 2020: 1-24. [paper](https://link.springer.com/article/10.1007/s11263-020-01369-0) [code](https://github.com/Jyouhou/SceneTextPapers)

**[90]** **\[ACM Computing Surveys-2020]** X. Chen, L. Jin, Y. Zhu, C. Luo, and T. Wang, “Text Recognition in the Wild: A Survey," ACM Computing Surveys (CSUR) 2020. [paper](https://arxiv.org/pdf/2005.03492.pdf) [code](https://github.com/HCIILAB/Scene-Text-Recognition)

***

<a id="4-ocr-service"></a>
## 4. OCR Service

|                             OCR                              | API  | Free | Code |
| :----------------------------------------------------------: | :--: | :--: | :--: |
| [Tesseract OCR Engine](https://github.com/tesseract-ocr/tesseract) |  ×   |  √   |  √   |
| [Azure](https://azure.microsoft.com/zh-cn/services/cognitive-services/computer-vision/#Analysis) |  √   |  √   |  ×   |
| [ABBYY](https://www.abbyy.cn/real-time-recognition-sdk/technical-specifications/) |  √   |  √   |  ×   |
|               [OCR Space](https://ocr.space/)                |  √   |  √   |  ×   |
|       [SODA PDF OCR](https://www.sodapdf.com/ocr-pdf/)       |  √   |  √   |  ×   |
|          [Free Online OCR](https://www.newocr.com/)          |  √   |  √   |  ×   |
|           [Online OCR](https://www.onlineocr.net/)           |  √   |  √   |  ×   |
|             [Super Tools](https://www.wdku.net/)             |  √   |  √   |  ×   |
|   [Online Chinese Recognition](http://chongdata.com/ocr/)    |  √   |  √   |  ×   |
|   [Calamari OCR](https://github.com/Calamari-OCR/calamari)   |  ×   |  √   |  √   |
| [ Tencent OCR](https://cloud.tencent.com/product/ocr?lang=cn) |  √   |  ×   |  ×   |

***

<a id="5-references"></a>
## 5. References

**[1] \[ICCV-2011]** K. Wang, B. Babenko, and S. Belongie, “End-to-end scene text recognition,” in Proceedings of ICCV, 2011, pp. 1457–1464. [paper ](https://www.researchgate.net/profile/Serge_Belongie/publication/221110077_End-to-end_scene_text_recognition/links/09e4150b34908d2ebb000000/End-to-end-scene-text-recognition.pdf)

**[2] \[BMVC-2012]** A. Mishra, K. Alahari, and C. Jawahar, “Scene text recognition using higher order language priors,” in Proceedings of BMVC, 2012, pp. 1–11. [paper](https://hal.inria.fr/hal-00818183/document) [dataset](http://cvit.iiit.ac.in/research/projects/cvit-projects/the-iiit-5k-word-dataset)

**[3] \[ICPR-2012]** T. Wang, D. J. Wu, A. Coates, and A. Y. Ng, “End-to-end text recognition with convolutional neural networks,” in Proceedings of ICPR, 2012, pp. 3304–3308. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6460871&tag=1)

**[4] \[ICDAR-2013]** V. Goel, A. Mishra, K. Alahari, and C. Jawahar, “Whole is greater than sum of parts: Recognizing scene text words,” in Proceedings of ICDAR, 2013, pp. 398–402. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6628652) 

**[5] \[ICCV-2013]** A. Bissacco, M. Cummins, Y. Netzer, and H. Neven, “Photoocr: Reading text in uncontrolled conditions,” in Proceedings of ICCV, 2013, pp. 785–792. [paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Bissacco_PhotoOCR_Reading_Text_2013_ICCV_paper.pdf)

**[6] \[ICCV-2013]** T. Quy Phan, P. Shivakumara, S. Tian, and C. Lim Tan, “Recognizing text with perspective distortion in natural scenes,” in Proceedings of ICCV, 2013, pp. 569–576. [paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Phan_Recognizing_Text_with_2013_ICCV_paper.pdf)

**[7] \[ICLR-2014]** O. Alsharif and J. Pineau, “End-to-end text recognition with hybrid HMM maxout models,” in Proceedings of ICLR: Workshop, 2014. [paper](https://arxiv.org/pdf/1310.1811.pdf)

**[8] \[TPAMI-2014]** J. Almaz ́an, A. Gordo, A. Forn ́ es, and E. Valveny, "Word spotting and recognition with embedded attributes,” IEEE Trans. Pattern Anal. Mach. Intell, vol. 36, no. 12, pp. 2552–2566, 2014. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6857995) [code](https://github.com/almazan/watts)

**[9] \[CVPR-2014]** C. Yao, X. Bai, B. Shi, and W. Liu, “Strokelets: A learned multiscale representation for scene text recognition,” in Proceedings of CVPR, 2014, pp. 4042–4049. [paper](http://openaccess.thecvf.com/content_cvpr_2014/papers/Yao_Strokelets_A_Learned_2014_CVPR_paper.pdf)

**[10] \[IJCV-2015]** J. A. Rodriguez-Serrano, A. Gordo, and F. Perronnin, “Label embedding: A frugal baseline for text recognition,” Int. J. Comput. Vis, vol. 113, no. 3, pp. 193–207, 2015. [paper](https://link.springer.com/content/pdf/10.1007%2Fs11263-014-0793-6.pdf)

**[11] \[ECCV-2014]** M. Jaderberg, A. Vedaldi, and A. Zisserman, “Deep features for text spotting,” in Proceedings of ECCV, 2014, pp. 512–528. [paper](https://link.springer.com/content/pdf/10.1007%2F978-3-319-10593-2_34.pdf) [code](https://bitbucket.org/jaderberg/eccv2014_textspotting/src/master/)

**[12] \[ACCV-2014]** B. Su and S. Lu, “Accurate scene text recognition based on recurrent neural network,” in Proceedings of ACCV, 2014, pp. 35–48. [paper](https://link.springer.com/content/pdf/10.1007%2F978-3-319-16865-4_3.pdf)

**[13] \[CVPR-2015]** A. Gordo, “Supervised mid-level features for word image representation,” in Proceedings of CVPR, 2015, pp. 2956–2964. [paper](http://openaccess.thecvf.com/content_cvpr_2015/papers/Gordo_Supervised_Mid-Level_Features_2015_CVPR_paper.pdf)

**[14] \[IJCV-2015]** M. Jaderberg, K. Simonyan, A. Vedaldi, and A. Zisserman, “Reading text in the wild with convolutional neural networks,” Int. J. Comput. Vis, vol. 116, no. 1, pp. 1–20, 2016. [paper](https://link.springer.com/content/pdf/10.1007%2Fs11263-015-0823-z.pdf) [code](http://www.robots.ox.ac.uk/~vgg/research/text/)

**[15] \[ICLR-2015]** M. Jaderberg, K. Simonyan, and A. Zisserman, “Deep structured output learning for unconstrained text recognition,” in Proceedings of ICLR, 2015. [paper](https://arxiv.org/pdf/1412.5903.pdf) 

**[16] \[TPAMI-2017]** B. Shi, X. Bai, and C. Yao, “An end-to-end trainable neural network for image-based sequence recognition and its application to scene text recognition,” IEEE Trans. Pattern Anal. Mach. Intell, vol. 39, no. 11, pp. 2298–2304, 2017. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7801919) [code-Torch7](https://github.com/bgshih/crnn) [code-Pytorch](https://github.com/meijieru/crnn.pytorch)

**[17] \[CVPR-2016]** B. Shi, X. Wang, P. Lyu, C. Yao, and X. Bai, “Robust scene text recognition with automatic rectification,” in Proceedings of CVPR, 2016, pp. 4168–4176. [paper](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Shi_Robust_Scene_Text_CVPR_2016_paper.pdf)

**[18] \[CVPR-2016]** C.-Y. Lee and S. Osindero, “Recursive recurrent nets with attention modeling for OCR in the wild,” in Proceedings of CVPR, 2016, pp. 2231–2239. [paper](http://openaccess.thecvf.com/content_cvpr_2016/papers/Lee_Recursive_Recurrent_Nets_CVPR_2016_paper.pdf)

**[19] \[BMVC-2016]** W. Liu, C. Chen, K.-Y. K. Wong, Z. Su, and J. Han, “STAR-Net: A spatial attention residue network for scene text recognition,” in Proceedings of BMVC, 2016, p. 7. [paper](https://i.cs.hku.hk/~kykwong/publications/wliu_bmvc16.pdf)

**[20] \[IJCAI-2017]** X. Yang, D. He, Z. Zhou, D. Kifer, and C. L. Giles, “Learning to read irregular text with attention mechanisms,” in Proceedings of IJCAI, 2017, pp. 3280–3286. [paper](https://pdfs.semanticscholar.org/1259/f7533abe2fe85fd9dead92853e2ff07a8792.pdf)

**[21] \[ICCV-2017]** F. Yin, Y.-C. Wu, X.-Y. Zhang, and C.-L. Liu, “Scene text recognition with sliding convolutional character models,” in Proceedings of ICCV, 2017. [paper](https://arxiv.org/pdf/1709.01727.pdf) [code](https://github.com/lsvih/Sliding-Convolution)

**[22] \[ICCV-2017]** Z. Cheng, F. Bai, Y. Xu, G. Zheng, S. Pu, and S. Zhou, “Focusing attention: Towards accurate text recognition in natural images,” in Proceedings of ICCV, 2017, pp. 5086–5094. [paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Cheng_Focusing_Attention_Towards_ICCV_2017_paper.pdf)

**[23] \[CVPR-2018]** Z. Cheng, Y. Xu, F. Bai, Y. Niu, S. Pu, and S. Zhou, “AON: Towards arbitrarily-oriented text recognition,” in Proceedings of CVPR, 2018, pp. 5571–5579. [paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Cheng_AON_Towards_Arbitrarily-Oriented_CVPR_2018_paper.pdf) [code](https://github.com/huizhang0110/AON)

**[24] \[NC-2019]** Y. Gao, Y. Chen, J. Wang, M. Tang, and H. Lu, “Reading scene text with fully convolutional sequence modeling,” Neurocomputing, vol. 339, pp. 161–170, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0925231219301870)

**[25] \[AAAI-2018]** W. Liu, C. Chen, and K.-Y. K. Wong, “Char-Net: A character-aware neural network for distorted scene text recognition.” in Proceedings of AAAI, 2018, pp. 7154–7161. [paper](https://i.cs.hku.hk/~kykwong/publications/wliu_aaai2018.pdf)

**[26] \[AAAI-2018]** Z. Liu, Y. Li, F. Ren, W. L. Goh, and H. Yu, “Squeezedtext: A real-time scene text recognition by binary convolutional encoderdecoder network,” in Proceedings of AAAI, 2018, pp. 7194–7201. [paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/16354/16312)

**[27] \[CVPR-2018]** F. Bai, Z. Cheng, Y. Niu, S. Pu, and S. Zhou, “Edit probability for scene text recognition,” in Proceedings of CVPR, 2018, pp. 1508–1516. [paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Bai_Edit_Probability_for_CVPR_2018_paper.pdf)

**[28] \[ECCV-2018]** Y. Liu, Z. Wang, H. Jin, and I. Wassell, “Synthetically supervised feature learning for scene text recognition,” in Proceedings of ECCV, 2018, pp. 449–465. [paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Yang_Liu_Synthetically_Supervised_Feature_ECCV_2018_paper.pdf)

**[29] \[ICIP-2018]** Y. Gao, Y. Chen, J. Wang, M. Tang, and H. Lu, “Dense chained attention network for scene text recognition,” in Proceedings of ICIP, 2018, pp. 679–683. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8451273)

**[30] \[TPAMI-2018]** B. Shi, M. Yang, X. Wang, P. Lyu, C. Yao, and X. Bai, “ASTER: An attentional scene text recognizer with flexible rectification,” IEEE Trans. Pattern Anal. Mach. Intell, vol. 41, no. 9, pp. 2035–2048, 2019. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8395027) [code](https://github.com/bgshih/aster)

**[31] \[CVPR-2012]** A. Mishra, K. Alahari, and C. Jawahar, “Top-down and bottom-up cues for scene text recognition,” in Proceedings of CVPR, 2012, pp. 2687–2694. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6247990)

**[32]** https://github.com/Canjie-Luo/MORAN_v2

**[33] \[ICDAR-2003]** S. M. Lucas, A. Panaretos, L. Sosa, A. Tang, S. Wong, and R. Young, “ICDAR 2003 robust reading competitions,” in Proceedings of ICDAR, 2003, pp. 682–687. [paper](https://link.springer.com/content/pdf/10.1007%2Fs10032-004-0134-3.pdf)

**[34] \[ICDAR-2013]** D. Karatzas, F. Shafait, S. Uchida, M. Iwamura, L. G. i Bigorda, S. R. Mestre, J. Mas, D. F. Mota, J. A. Almazan, and L. P. De Las Heras, “ICDAR 2013 robust reading competition,” in Proceedings of ICDAR, 2013, pp. 1484–1493. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6628859)

**[35] \[ICCV-2013]** T. Quy Phan, P. Shivakumara, S. Tian, and C. Lim Tan, “Recognizing text with perspective distortion in natural scenes,” in Proceedings of ICCV, 2013, pp. 569–576. [paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Phan_Recognizing_Text_with_2013_ICCV_paper.pdf)

**[36] \[Expert Syst.Appl-2014]** A. Risnumawan, P. Shivakumara, C. S. Chan, and C. L. Tan, “A robust arbitrary text detection system for natural scene images,” Expert Systems with Applications, vol. 41, no. 18, pp. 8027–8048, 2014. [paper](https://pdf.sciencedirectassets.com/271506/1-s2.0-S0957417414X00114/1-s2.0-S0957417414004060/main.pdf?x-amz-security-token=AgoJb3JpZ2luX2VjEIn%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJGMEQCIGRhldIzSEiSi38FQg8SKy0nbkjetbYc6MOZN8lXbsg7AiB5pY6PoVDS8%2F3qS%2FPqd0zaHjqWrjqvDrAtTiZVSrpKmyrjAwiC%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAIaDDA1OTAwMzU0Njg2NSIMoRUcs%2Ft3M%2Blz7DI3KrcDKVODcJNpq1tNel77UHdAJVSUDWRkG7Fx5loyHhQsb2V3MFfHqAGKJpbdr7xHlDY7CaTl5nrTdNe91InXfpM25fFyYQlANwrhlcYGiPEsN14mSBe%2F5gy0gipiPaN835Viwb0O1Raw9MP9Clc84q%2BHvW5YyQ02NIZYE7OlHYSWN6mbI0F9r7reRa2zNLjFVcvJRkAyt4I9L1Pbehf4WwFF1Er0ResczdJ2FbwKCZNaKWznwhdjVp8hw0SFC%2F9uxnDHzu8DTPeutA3mHeUetMOEtKspkSvIj%2FWQDI1OTECcNv0N7CfmUKSh9m5tOYn%2Fb7KQx8pPA450Snd3faB7euDzPwvCmtfeUzYs0n0UxWt9JWXxKONmvrMlxf9bjZL0RBR1NNeNgwFuCCCRZDAKogbBI%2FclJmPUiNO38mHO10B1unMow9XtojodS3U6Iz2n8jeERhaR4Rt4KeWB9ojZTQhUr5d1uUX%2FVpmJmFQhgvPXmEi%2Fnlp65TXeZNdbUncQPqZ8PaKGYxJn1F%2FwnuJH1Ww6ksTur4rcggGAEHTBgXL5vmLjJG2ZhH1vxaoY8qtUO5EuXwVVfBXCtzCit9jmBTq1Abb%2BixDckXLEYAwidBhA%2B4MKpbhmH4LItnjE3tSuFgOHFbwaq9g0MZyGtL3OUxCKc3eAkkLzOrJnEag%2F2eV%2BdMcU9%2F%2BKI5h8yQsz5PEFeqkY3BID%2BY7oIU6qhqhb38PVrbt1oyF420cS%2BoSpt2Nj6E%2FuCZZTrgMakE%2B9QXvAaTIBWG%2Fc0xOv6d3rGTAnZTkkscgD7j%2FP1jqFkf388YT5jCbAWlx8OiMbj%2BVPkK8UvXhgSh1ZPMk%3D&AWSAccessKeyId=ASIAQ3PHCVTY6VYAY5FB&Expires=1557539079&Signature=HF7E%2BOACBDJPtLAerMWH6MTKDCw%3D&hash=8fe7c8a1c5599e4659a2b26919b2a59f4aff8c452e5a07793dc187e49c69dc9e&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0957417414004060&tid=spdf-7bd6a860-4c57-4e39-87ce-bd2f050badcf&sid=57f9f09d5d026341242a7bd2fb38b97c5897gxrqb&type=client)

**[37] \[ICDAR-2015]** D. Karatzas, L. Gomez-Bigorda, A. Nicolaou, S. Ghosh, A. Bagdanov, M. Iwamura, J. Matas, L. Neumann, V. R. Chandrasekhar, S. Lu et al., “ICDAR 2015 competition on robust reading,” in Proceedings of ICDAR, 2015, pp. 1156–1160. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7333942)

**[38] \[arXiv-2016]** A. Veit, T. Matera, L. Neumann, J. Matas, and S. Belongie, “Coco-text: Dataset and benchmark for text detection and recognition in natural images,” CoRR abs/1601.07140, 2016. [paper](https://arxiv.org/pdf/1601.07140.pdf) [code](https://github.com/andreasveit/coco-text)

**[39] \[IJDAR-2019]** C.-K. Ch’ng, C. S. Chan, and C.-L. Liu, “Total-text: toward orientation robustness in scene text detection,” International Journal on Document Analysis and Recognition (IJDAR), pp. 1–22, 2019. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8270088) [code](https://github.com/cs-chan/Total-Text-Dataset)

**[40] \[ICDAR-2017]** B. Shi, C. Yao, M. Liao, M. Yang, P. Xu, L. Cui, S. Belongie, S. Lu, and X. Bai, “ICDAR2017 competition on reading chinese text in the wild (rctw-17),” in Proceedings of ICDAR, 2017, pp. 1429–1434. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8270164)

**[41] \[ICPR-2018]** M. He, Y. Liu, Z. Yang, S. Zhang, C. Luo, F. Gao, Q. Zheng, Y. Wang, X. Zhang, and L. Jin, “ICPR2018 contest on robust reading for multi-type web images,” in Proceedings of ICPR, 2018, pp. 7–12. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8546143)

**[42] \[JCS&T-2019]** Yuan T L, Zhu Z, Xu K, et al. A large chinese text dataset in the wild[J]. Journal of Computer Science and Technology, 2019, 34(3): 509-521. [paper](https://link.springer.com/article/10.1007/s11390-019-1923-y) [code](https://github.com/yuantailing/ctw-baseline)

**[43] \[arXiv-2017]** L. Yuliang, J. Lianwen, Z. Shuaitao, and Z. Sheng, “Detecting curve text in the wild: New dataset and new solution,” CoRR abs/1712.02170, 2017. [paper](https://arxiv.org/pdf/1712.02170.pdf) [code](https://github.com/Yuliang-Liu/Curve-Text-Detector)

**[44] \[ECCV-2018]** P. Lyu, M. Liao, C. Yao, W. Wu, and X. Bai, “Mask textspotter: An end-to-end trainable neural network for spotting text with arbitrary shapes,” in Proceedings of ECCV, 2018, pp. 67–83. [paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Pengyuan_Lyu_Mask_TextSpotter_An_ECCV_2018_paper.pdf) [code](https://github.com/lvpengyuan/masktextspotter.caffe2)

**[45] \[NIPS-W-2011]** Y. Netzer, T. Wang, A. Coates, A. Bissacco, B. Wu, and A. Y. Ng, “Reading digits in natural images with unsupervised feature learning,” in Proceedings of NIPS, 2011. [paper](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/37648.pdf)

**[46] \[PR-2019]**  C. Luo, L. Jin, and Z. Sun, “MORAN: A multi-object rectified attention network for scene text recognition,” Pattern Recognition, vol. 90, pp. 109–118, 2019. [paper](https://pdf.sciencedirectassets.com/272206/1-s2.0-S0031320319X00023/1-s2.0-S0031320319300263/main.pdf?x-amz-security-token=AgoJb3JpZ2luX2VjEHcaCXVzLWVhc3QtMSJIMEYCIQCceDsmz9xCoE%2FnPRGjEfK6RAdvbVW7B%2B7rvG4viZPq%2BAIhALnS8lFI9N7LE3%2BNey3EgbWZU8f%2BJIAJIxlk5ewtKNTgKtoDCG8QAhoMMDU5MDAzNTQ2ODY1IgxbFmRrlDI1X0pjiscqtwMyG%2F2gaQjY2Ol3wnc2MtQwmfUOBotnxAj7F7lPnLyeRqPWJo6swI52Tz0YWuSI%2FTXRk3wuLNZthvTkLRWlD5wejFNGIAM9VNUuaYmfhLPT%2Ft33yaDBMGBe3wP%2BdsH0OXHn7JtbzLAFK%2BFPBYXLfSMth4IbmdKzLPAR77noWqY3NvtbYRJEvpw4r9N7yvM%2Fo1lBQnoulBsX%2B7sKRKm9SxWrreldzSuX2EIbnk5FPyXAkTlzYfH%2FCjoTOGYrReZl1VeFSnml73TaF1RImYbO0t155QfM8X90oEMKxlfd1IU8PzuYy14%2Bo0TAmHB3kYh3aKN6CEZ%2FEAHhxxhGrysEhBZWLF0RMp2oZFGDPxiOJVo3QES2GR38d9uBYjXF0dzjxgFnn40SuYTRE29nIjspgjZbsqeWyP%2BbsFHJcteX3w0eN6wq%2B%2Bbd5yPuAELoAy246KPZvRwBXGYUH1%2Bgm%2BqIIKidMGUedx98L2%2FO%2FAnbQ7gPCKW9HIWRdExufStWHid2r8gPpwB3%2Fb%2FKtCbA7iqm7cedZaqgjvaBbKM0hgBlgfXMGJTniXSmGYAIhvgH0aAlUCAAGeNsovbGMMCw1OYFOrMBESogEL75zcwF5QSaTC8s2DdSVFWjhwza7lgexCXY7r6aW4Y80XYluSj6%2BPWj2x6qH23kIlPIEfmyXL%2FJbbBzxTh%2FBbA9UVu04wph8eB%2BNGtvajIx%2FZFVNJSHc3WHz2DWlSAkLnuNGtahDLdXTG3ZD9jhdbweN7QdKYXsPPLh6ysos7v0hO9f7mM2%2BWsA5yOwB8lg9d2xmYu2PU6RKCQcv8hC1ASHgZh5PiYGBUjTfdv0cfI%3D&AWSAccessKeyId=ASIAQ3PHCVTYXA3CRTFK&Expires=1557473755&Signature=eBwdaj8gPpxtBnisCTPveLqX3iw%3D&hash=6f612616f8fba56ffd779d1eee8bfb19e39b7276f2b922ed529a46e51075049d&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0031320319300263&tid=spdf-5d02711b-ea3c-46c1-bb55-4d301d13f947&sid=57f9f09d5d026341242a7bd2fb38b97c5897gxrqb&type=client) [code](https://github.com/Canjie-Luo/MORAN_v2)

**[47] \[ACM-2019]** Xie H, Fang S, Zha Z J, et al, “Convolutional Attention Networks for Scene Text Recognition,” ACM Transactions on Multimedia Computing, Communications, and Applications (TOMM), vol. 15, pp. 3 2019. [paper](https://dl.acm.org/citation.cfm?id=3231737)

**[48] \[AAAI-2019]** M. Liao, J. Zhang, Z. Wan, F. Xie, J. Liang, P. Lyu, C. Yao, and X. Bai, “Scene text recognition from two-dimensional perspective,” in Proceedings of AAAI, 2019, pp. 8714–8721. [paper](https://arxiv.org/pdf/1809.06508.pdf) 

**[49] \[AAAI-2019]** H. Li, P. Wang, C. Shen, and G. Zhang, “Show, attend and read: A simple and strong baseline for irregular text recognition,” in Proceedings of AAAI, 2019, pp. 8610–8617. [paper](https://arxiv.org/pdf/1811.00751.pdf) [code](https://tinyurl.com/ShowAttendRead)

**[50] \[TPAMI-2015]** Q. Ye and D. Doermann, “Text detection and recognition in imagery: A survey,” IEEE Trans. Pattern Anal. Mach. Intell, vol. 37, no. 7, pp. 1480–1500, 2015. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6945320)

**[51] \[Frontiers-Comput. Sci-2016]** Y. Zhu, C. Yao, and X. Bai, “Scene text detection and recognition: Recent advances and future trends,” Frontiers of Computer Science, vol. 10, no. 1, pp. 19–36, 2016. [paper](https://link.springer.com/article/10.1007/s11704-015-4488-0)

**[52] \[IJCV-2020]**  Long S, He X, Yao C. Scene text detection and recognition: The deep learning era[J]. International Journal of Computer Vision, 2020: 1-24. [paper](https://link.springer.com/article/10.1007/s11263-020-01369-0) [code](https://github.com/Jyouhou/SceneTextPapers)

**[53] \[NIPS-W-2014]** M. Jaderberg, K. Simonyan, A. Vedaldi, and A. Zisserman, “Synthetic data and artificial neural networks for natural scene text recognition,” in Proceedings of NIPS-W, 2014. [paper](https://arxiv.org/pdf/1406.2227.pdf) [code](http://www.robots.ox.ac.uk/~vgg/publications/2014/Jaderberg14c/)

**[54] \[CVPR-2016]** A. Gupta, A. Vedaldi, and A. Zisserman, “Synthetic data for text
localisation in natural images,” in Proceedings of CVPR, 2016, pp. 2315–2324. [paper](http://www.robots.ox.ac.uk/~ankush/textloc.pdf) [code](https://github.com/ankush-me/SynthText)

**[55] \[CVPR-2019]** F. Zhan and S. Lu, “ESIR: End-to-end scene text recognition via iterative image rectification,” in Proceedings of CVPR, 2019, pp. 2059–2068. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhan_ESIR_End-To-End_Scene_Text_Recognition_via_Iterative_Image_Rectification_CVPR_2019_paper.pdf)

**[56] \[CVPR-2019]** Y. Zhang, S. Nie, W. Liu, X. Xu, D. Zhang, and H. T. Shen, “Sequence-to-sequence domain adaptation network for robust text image recognition,” in Proceedings of CVPR, 2019, pp. 2740–2749. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_Sequence-To-Sequence_Domain_Adaptation_Network_for_Robust_Text_Image_Recognition_CVPR_2019_paper.pdf) [code](https://github.com/AprilYapingZhang/Seq2SeqAdapt)

**[57]\[ICDAR-2019]** Y. Sun, Z. Ni, C.-K. Chng, Y. Liu, C. Luo, C. C. Ng, J. Han, E. Ding, J. Liu, D. Karatzas et al., “ICDAR 2019 competition on large-scale street view text with partial labeling–RRC-LSVT,” in Proceedings of ICDAR, 2019, pp. 1557–1562. [paper](https://arxiv.org/abs/1909.07741) [Link](https://rrc.cvc.uab.es/?ch=16)

**[58]\[ICDAR-2019]** C.-K. Chng, Y. Liu, Y. Sun, C. C. Ng, C. Luo, Z. Ni, C. Fang, S. Zhang, J. Han, E. Ding et al., “ICDAR2019 robust reading challenge on arbitrary-shaped text (RRC-ArT),” in Proceedings of ICDAR, 2019, pp. 1571–1576. [paper](https://arxiv.org/pdf/1909.07145.pdf) [Link](https://rrc.cvc.uab.es/?ch=14) 

**[59]\[ICDAR-2019]** X. Liu, R. Zhang, Y. Zhou, Q. Jiang, Q. Song, N. Li, K. Zhou, L. Wang, D. Wang, M. Liao et al., “ICDAR 2019 robust reading challenge on reading chinese text on signboard,” in Proceedings of ICDAR, 2019, pp. 1577–1581. [paper](https://ieeexplore.ieee.org/abstract/document/8978135) [Link](https://rrc.cvc.uab.es/?ch=12)

**[60] \[NC-2019]**  X. Chen, T. Wang, Y. Zhu, L. Jin, and C. Luo, “Adaptive embedding gate for attention-based scene text recognition,” Neurocomputing, vol. 381, pp. 261–271, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0925231219316510)

***

**Newly added references (Dec 24, 2019)**

**[61]** **\[ICFHR-2018]** C. Wang, F. Yin, and C.-L. Liu, “Memory-augmented attention model for scene text recognition,” in Proceedings of ICFHR, 2018, pp. 62–67.  [paper](https://ieeexplore.ieee.org/abstract/document/8563227)

**[62]** **\[ICCV-2019]** M. Yang, Y. Guan, M. Liao, X. He, K. Bian, S. Bai, C. Yao, and X. Bai, “Symmetry-constrained rectification network for scene text recognition,” in Proceedings of ICCV, 2019, pp. 9147–9156. [paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Yang_Symmetry-Constrained_Rectification_Network_for_Scene_Text_Recognition_ICCV_2019_paper.pdf)

**[63]** **\[ICCV-2019]** Y. Sun, J. Liu, W. Liu, J. Han, E. Ding, and J. Liu, “Chinese street view text: Large-scale chinese text reading with partially supervised learning,” in Proceedings of ICCV, 2019, pp. 9086–9095. [paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Sun_Chinese_Street_View_Text_Large-Scale_Chinese_Text_Reading_With_Partially_ICCV_2019_paper.pdf)

**[64]** **\[ICME-2019]** S. Wang, Y. Wang, X. Qin, Q. Zhao, and Z. Tang, “Scene text recognition via gated cascade attention,” in Proceedings of ICME, 2019, pp. 1018–1023. [paper](https://ieeexplore.ieee.org/abstract/document/8784914)

**[65]** **\[ICCV-2019]** J. Baek, G. Kim, J. Lee, S. Park, D. Han, S. Yun, S. J. Oh, and H. Lee, “What is wrong with scene text recognition model comparisons? dataset and model analysis,” in Proceedings of ICCV, 2019, pp. 4714–4722. [paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Baek_What_Is_Wrong_With_Scene_Text_Recognition_Model_Comparisons_Dataset_ICCV_2019_paper.pdf) [code](https://github.com/clovaai/deep-text-recognition-benchmark)

**[66]** **\[Nips-2017]** J. Wang and X. Hu, “Gated recurrent convolution neural network
for OCR,” in Proceedings of NIPS, 2017, pp. 335–344. [paper](http://papers.nips.cc/paper/6637-gated-recurrent-convolution-neural-network-for-ocr.pdf) [code](https://github.com/Jianfeng1991/GRCNN-for-OCR)

**[67]** **\[NC-2020]** Y. Huang, Z. Sun, L. Jin, and C. Luo, “EPAN: Effective parts attention network for scene text recognition,” Neurocomputing, vol. 376, pp. 202–213, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0925231219313839)

**[68]** **\[NC-2019]** Y. Gao, Y. Chen, J. Wang, M. Tang, and H. Lu, “Reading scene text with fully convolutional sequence modeling,” Neurocomputing, vol. 339, pp. 161–170, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S0925231219301870)

**[69]** **\[ICDAR-W-2019]** X. Qi, Y. Chen, R. Xiao, C.-G. Li, Q. Zou, and S. Cui, “A novel joint character categorization and localization approach for characterlevel scene text recognition,” in Proceedings of ICDAR: Workshops, 2019, pp. 83–90. [paper](https://ieeexplore.ieee.org/abstract/document/8892915)

**[70]** **\[ICDAR-W-2019]** Q. Wang, W. Jia, X. He, Y. Lu, M. Blumenstein, Y. Huang, and S. Lyu, “ReELFA: A scene text recognizer with encoded location and focused attention,” in Proceedings of ICDAR: Workshops, 2019, pp. 71–76. [paper](https://ieeexplore.ieee.org/abstract/document/8892900)

**[71]** **\[ICIP-2019]** Y. Zhu, S. Wang, Z. Huang, and K. Chen, “Text recognition in images based on transformer with hierarchical attention,” in Proceedings of ICIP, 2019, pp. 1945–1949. [paper](https://ieeexplore.ieee.org/abstract/document/8803203)

**[72]** **\[CVPR-2019]** F. Zhan, H. Zhu, and S. Lu, “Spatial fusion gan for image synthesis,” in Proceedings of CVPR, 2019, pp. 3653–3662. [paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhan_Spatial_Fusion_GAN_for_Image_Synthesis_CVPR_2019_paper.pdf)

**[73]** **\[ECCV-2018]** F. Zhan, S. Lu, and C. Xue, “Verisimilar image synthesis for accurate detection and recognition of texts in scenes,” in Proceedings of ECCV, 2018, pp. 249–266. [paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Fangneng_Zhan_Verisimilar_Image_Synthesis_ECCV_2018_paper.pdf) [code](https://github.com/fnzhan/Verisimilar-Image-Synthesis-for-Accurate-Detection-and-Recognition-of-Texts-in-Scenes)

**[74]** **\[MultiMedia-2018]** S. Fang, H. Xie, Z.-J. Zha, N. Sun, J. Tan, and Y. Zhang, “Attention and language ensemble for scene text recognition with convolutional sequence modeling,” in ACM Multimedia Conference on Multimedia Conference, 2018, pp. 248–256. [paper](https://dl.acm.org/citation.cfm?id=3240571) [code](https://github.com/FangShancheng/conv-ensemble-str)

**[75]** **\[Nips-2018]** H. Liu, S. Jin, and C. Zhang, “Connectionist temporal classification with maximum entropy regularization,” in Proceedings of NIPS, 2018, pp. 831–841 . [paper](http://papers.nips.cc/paper/7363-connectionist-temporal-classification-with-maximum-entropy-regularization) [code](https://github.com/liuhu-bigeye/enctc.crnn )

**[76]** **\[PR-2017]** B. Su and S. Lu, “Accurate recognition of words in scenes without
character segmentation using recurrent neural network,” Pattern Recognition, vol. 63, pp. 397–405, 2017. [paper](https://www.sciencedirect.com/science/article/pii/S0031320316303314)

**[77]** **\[CVIU-2016]** A. Mishra, K. Alahari, and C. Jawahar, “Enhancing energy minimization framework for scene text recognition with top-down cues,” Computer Vision and Image Understanding, vol. 145, pp. 30–42, 2016. [paper](https://www.sciencedirect.com/science/article/pii/S107731421600014X)

**[78]** **\[ICPR-2016]** X. Liu, T. Kawanishi, X. Wu, and K. Kashino, “Scene text recognition with CNN classifier and WFST-based word labeling,” in Proceedings of ICPR, 2016, pp. 3999–4004. [paper](https://ieeexplore.ieee.org/abstract/document/7900259)  

**[79]** **\[TPAMI-2019]** M. Liao, P. Lyu, M. He, C. Yao, W. Wu, and X. Bai, “Mask textspotter: An end-to-end trainable neural network for spotting text with arbitrary shapes,” IEEE Trans. Pattern Anal. Mach. Intell, 2019. [paper](https://ieeexplore.ieee.org/abstract/document/8812908) [code](https://github.com/MhLiao/MaskTextSpotter)

**[80]** **\[AAAI-2020]** T. Wang, Y. Zhu, L. Jin, C. Luo, X. Chen, Y. Wu, Q. Wang, and M. Cai, “Decoupled attention network for text recognition,” in Proceedings of AAAI, 2020. [paper](https://arxiv.org/pdf/1912.10205.pdf) [code](https://github.com/Wang-Tianwei/Decoupled-attention-network)

---

**Newly added references (Feb 29, 2020)**

**[81]** **\[ICDAR-2019]** N. Nayef, Y. Patel, M. Busta, P. N. Chowdhury, D. Karatzas, W. Khlif, J. Matas, U. Pal, J.-C. Burie, C.-l. Liu et al., “ICDAR2019 robust reading challenge on multi-lingual scene text detection and recognition–RRC-MLT-2019,” in Proceedings of ICDAR, 2019, pp. 1582–1587. [paper](https://arxiv.org/pdf/1907.00945.pdf)

**[82]** **\[arXiv-2019]** W. Wang, E. Xie, P. Sun, W. Wang, L. Tian, C. Shen, and P. Luo, “TextSR: Content-aware text super-resolution guided by recognition,” CoRR abs/1909.07113, 2019. [paper](https://arxiv.org/pdf/1909.07113.pdf) [code](https://github.com/xieenze/TextSR)

**[83]** **\[AAAI-2020]** Z. Wan, M. He, H. Chen, X. Bai, and C. Yao, “Textscanner: Reading characters in order for robust scene text recognition,” In Proceedings of AAAI, 2020. [paper](https://arxiv.org/pdf/1912.12422.pdf) 

**[84]** **\[AAAI-2020]** W. Hu, X. Cai, J. Hou, S. Yi, and Z. Lin, “GTC: Guided training of ctc towards efficient and accurate scene text recognition,” In Proceedings of AAAI, 2020. [paper](https://www.aaai.org/Papers/AAAI/2020GB/AAAI-HuW.7838.pdf) 

**[85]** **\[IJCV-2020]** C. Luo, Q. Lin, Y. Liu, J. Lianwen, and S. Chunhua, “Separating content from style using adversarial learning for recognizing text in the wild,” Int. J. Comput. Vis. 2020. [paper](https://arxiv.org/pdf/2001.04189.pdf) 

---

**Newly added references (May 8, 2020)**

**[86]** **\[CVPR-2020]** R. Litman, O. Anschel, S. Tsiper, R. Litman, S. Mazor, and R. Manmatha, “SCATTER: selective context attentional scene text recognizer,” in Proceedings of CVPR, 2020. [paper](https://arxiv.org/abs/2003.11288.pdf) 

**[87]** **\[CVPR-2020]**  D. Yu, X. Li, C. Zhang, J. Han, J. Liu, and E. Ding, “Towards accurate scene text recognition with semantic reasoning networks,” in Proceedings of CVPR, 2020. [paper](https://arxiv.org/abs/2003.12294.pdf) 

**[88]** **\[CVPR-2020]** S. Long and C. Yao, “UnrealText: Synthesizing realistic scene text images from the unreal world,” in Proceedings of CVPR, 2020. [paper](https://arxiv.org/abs/2003.10608.pdf)

**[89]** **\[ECCV-2016]** W. Qiu and A. L. Yuille, “Unrealcv: Connecting computer vision
to unreal engine,” in Proceedings of ECCV, 2016, pp. 909–916. [paper](https://link.springer.com/chapter/10.1007/978-3-319-49409-8_75)

**[90]** **\[ACM Computing Surveys-2020]** X. Chen, L. Jin, Y. Zhu, C. Luo, and T. Wang, “Text Recognition in the Wild: A Survey," ACM Computing Surveys (CSUR) 2020. [paper](https://arxiv.org/pdf/2005.03492.pdf) [code](https://github.com/HCIILAB/Scene-Text-Recognition)

---

**Newly added references (Dec 8, 2020)**

**[91]** **\[ICVGIP-2018]** Gupta A, Vedaldi A, Zisserman A. "Learning to read by spelling: Towards unsupervised text recognition," in Proceedings of ICVGIP, 2018. [paper](https://dl.acm.org/doi/pdf/10.1145/3293353.3293386) 

**[92]** **\[CVPR-2020]** Wan Z, Zhang J, Zhang L, et al, "On Vocabulary Reliance in Scene Text Recognition," in  Proceedings of CVPR, 2020. [paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Wan_On_Vocabulary_Reliance_in_Scene_Text_Recognition_CVPR_2020_paper.pdf) 

**[93]** **\[ECAI-2020]** Bleeker M, de Rijke M, "Bidirectional Scene Text Recognition with a Single Decoder," in Proceedings of ECAI, 2020. [paper](https://arxiv.org/pdf/1912.03656.pdf) [code](https://github.com/MauritsBleeker/Bi-STET)

**[94]** **\[arXiv-2019]** Bartz C, Bethge J, Yang H, et al, "KISS: Keeping It Simple for Scene Text Recognition,"CoRR abs/1911.08400, 2019. [paper](https://arxiv.org/pdf/1911.08400.pdf) [code](https://github.com/Bartzi/kiss)

**[95]** **\[arXiv-2020]**  Zhang C, Xu Y, Cheng Z, et al, "SPIN: Structure-Preserving Inner Offset Network for Scene Text Recognition,"  CoRR abs/2005.13117, 2020. [paper](https://arxiv.org/pdf/2005.13117.pdf) 

**[96]** **\[arXiv-2020]**  Lin J, Cheng Z, Bai F, et al, "Text Recognition in Real Scenarios with a Few Labeled Samples,"  CoRR abs/2006.12209, 2020. [paper](https://arxiv.org/pdf/2006.12209.pdf) 

**[97]** **\[ECCV-2020]**  Zhang C, Gupta A, Zisserman A. "Adaptive Text Recognition through Visual Matching," in Proceedings of ECCV, 2020. [paper](https://link.springer.com/chapter/10.1007/978-3-030-58517-4_4)  [code]( http://www.robots.ox.ac.uk/~vgg/research/FontAdaptor20/)

**[98]** **\[ECCV-2020]**  Zhang H, Yao Q, Yang M, et al, "AutoSTR: Efficient Backbone Search for Scene Text Recognition," in Proceedings of ECCV, 2020. [paper](http://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123690732.pdf)  [code](https://github.com/AutoML-4Paradigm/AutoSTR.git)

**[99]** **\[ECCV-2020]**   Yan R, Huang Y, "PlugNet: Degradation Aware Scene Text Recognition Supervised by a Pluggable Super-Resolution Unit," in Proceedings of ECCV, 2020. [paper](http://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123600154.pdf) 

**[100]** **\[ECCV-2020]**   Yue X, Kuang Z, Lin C, et al. RobustScanner: Dynamically Enhancing Positional Clues for Robust Text Recognition," in Proceedings of ECCV, 2020. [paper](https://arxiv.org/pdf/2007.07542.pdf) 

**[101]** **\[CVPR-2020]**   Zhi Qiao, Yu Zhou, Dongbao Yang, Yucan Zhou, and Weiping Wang. 2020. SEED: Semantics Enhanced Encoder-Decoder Framework for Scene Text Recognition. In Proceedings of CVPR. [paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Qiao_SEED_Semantics_Enhanced_Encoder-Decoder_Framework_for_Scene_Text_Recognition_CVPR_2020_paper.pdf) [code]( https://github.com/Pay20Y/SEED)

<a id="6help"></a>

## 6.Help

If you have any problem in our resources, or any good paper/code we missed, please inform us at xxuechen@foxmail.com. Thank you for your contribution.

***

<a id="7copyright"></a>

<a id="7copyright"></a>
## 7.Copyright

Copyright © 2020 SCUT-DLVC. All Rights Reserved.

<p align="center">
    <img src="scut-dlvc.jpeg" alt="Sample"  width="150" height="75">
    <p align="center">
        <em></em>
    </p>
</p>
