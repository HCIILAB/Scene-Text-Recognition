# Scene Text Recognition Resources 
[Chinese_version](/scene_text_recognition_chinese_version.md)

[<p align='right'>Author:陈晓雪</p>](https://github.com/CCchenxiaoxue)
<!-- MarkdownTOC -->

1. [1. Datasets](#1-datasets)
    1. [1.1 Regular Scene Text Datasets](#11-regular-scene-text-datasets)
    1. [1.2 Irregular Scene Text Datasets](#12-irregular-scene-text-datasets)
    1. [1.3 Chinese Scene Text Datasets](#13-chinese-scene-text-datasets)
    1. [1.4 Synthetic Datasets](#14-synthetic-datasets)
    1. [1.5 Comparison of Datasets](#15-comparison-of-datasets)
1. [2. Summary of Scene Text Recognition Results](#2-summary-of-scene-text-recognition-results)
    1. [2.1 Introduction](#21-introduction)
    1. [2.2 Summary of Scene Text Recognition Results](#22-summary-of-scene-text-recognition-results)
    1. [2.3 Chinese Scene Text Recognition Results](#23-chinese-scene-text-recognition-results)
1. [3. Field Survey](#3-field-survey)
1. [4. OCR Service](#4-ocr-service)
1. [5. References](#5-references)

<!-- /MarkdownTOC -->

***

<a id="1-datasets"></a>

<a id="1-datasets"></a>
## 1. Datasets

<a id="11-regular-scene-text-datasets"></a>
### 1.1 Regular Scene Text Datasets

- IIIT5K[31]：
  * **Introduction:** There are 5000 images in total, 2000 for training and 3000 for testing. Text instances are mostly horizontal. Each image is associated with a short, 50-word lexicon and a long, 1000-word lexicon. (The lexicon consists of the groundtruth word and other random words.)
  * **Link:** [IIIT5K-download](http://cvit.iiit.ac.in/research/projects/cvit-projects/the-iiit-5k-word-dataset)
- SVT[32]：
  * **Introduction:** There are 647 images of cropped words. Text instances are mostly horizontal. Many images are severely corrupted by noise, blur, and low resolution. SVT is collected from the Google Street View, and each image is associated with a 50-word lexicon. It only has word-level annotations.
  * **Link:** [SVT-download](http://vision.ucsd.edu/~kai/grocr/)
- ICDAR 2003(IC03)[33]：
  * **Introduction:** There are 509 images in total, 258 for training and 251 for testing. It contains 867 test images of cropped word after filtering. Text instances are mostly horizontal. Each image is associated with a 50-word lexicon and a full-word lexicon.  (The full lexicon combines all lexicon words.)
  * **Link:** [IC03-download](http://www.iapr-tc11.org/mediawiki/index.php?title=ICDAR_2003_Robust_Reading_Competitions)
- ICDAR 2013(IC13)[34]：
  * **Introduction:** There are 1015 images of cropped word. Most images of IC13 are inherits from IC03. The text are mostly horizontal. No lexicon is provided.
  * **Link:** [IC13-download](http://dagdata.cvc.uab.es/icdar2013competition/?ch=2&com=downloads)
- SVHN[45]：
  * **Introduction:** There are 600000 digits of house numbers in natural scenes. The digits are mostly horizontal. SVHN is collected from the Google View images, and is used to digit recognition.
  * **Link:** [SVHN-download](http://ufldl.stanford.edu/housenumbers/)

<a id="12-irregular-scene-text-datasets"></a>
### 1.2 Irregular Scene Text Datasets

- SVT-P[35]：
  - **Introduction:** There are 639 images of cropped word. Many images are heavily distorted by the non-frontal view angle. SVT-P is collected from the side-view images in Google Street View. Each image is associated with a 50-word lexicon and a full-word lexicon.
  - **Link:** [SVT-P-download](https://pan.baidu.com/s/1rhYUn1mIo8OZQEGUZ9Nmrg )  \(Extraction code : vnis)
- CUTE80[36]：
  - **Introduction:** There are 80 high-resolution images taken in natural scenes. It contains 288 test images of cropped word after filtering and focuses on curved text. No lexicon is provided.
  - **Link:** [CUTE80-download](http://cs-chan.com/downloads_CUTE80_dataset.html)
- ICDAR 2015(IC15)[37]：
  - **Introduction:** There are 1500 images in total, 1000 for training and 500 for testing. It contains 2077 test images of cropped word including more than 200 irregular text. No lexicon is provided.
  - **Link:** [IC15-download](http://rrc.cvc.uab.es/?ch=4&com=downloads)
- COCO-Text[38]：
  - **Introduction:** There are 63686 images in total. It contains 145859 test images of cropped word including handwritten and printed, clear and blur, English and non-English.
  - **Link:** [COCO-Text-download](https://vision.cornell.edu/se3/coco-text-2/)
- Total-Text[39]：
  - **Introduction:** There are 1555 images in total. It contains 11459 test images of cropped word with more than three different text orientations: horizontal, multi-oriented and curved.
  - **Link:** [Total-Text-download](https://github.com/cs-chan/Total-Text-Dataset)
- CTW-1500[43]：
  - **Introduction:** There are 1500 images in total, 1000 for training and 500 for testing. It contains 10751 test images of cropped word. Text instances are multi-oriented and curved. The main languages are Chinese and English.
  - **Link:** [CTW-1500-download](https://github.com/Yuliang-Liu/Curve-Text-Detector)

<a id="13-chinese-scene-text-datasets"></a>
### 1.3 Chinese Scene Text Datasets

- CTW-12k(RCTW competition，ICDAR17)[40]：
  - **Introduction:** There are 12514 images in total, 11514 for training and 1000 for testing. Most images in CTW-12k is collected by camera or mobile phone, and others are generated images. Each image contains more than one text line. The competition tasks include text detection and end-to-end text recognition.
  - **Link:** [CTW-12K-download](http://rctw.vlrlab.net/dataset/)
- MTWI(competition)[41]：
  - **Introduction:** There are 20000 images. Text instances are mainly Chinese or English web text. The competition tasks include web text recognition, web text detection and end-to-end web text detection and recognition.
  - **Link:** [MTWI-download ](https://pan.baidu.com/s/1SUODaOzV7YOPkrun0xSz6A#list/path=%2F)  \(Extraction code:gox9)
- CTW[42]：
  - **Introduction:** There are 32285 high resolution street view images of Chinese text, with 1018402 character instances in total. CTW contains planar text, text in cities, text in rural areas, text under poor illumination, distant text, partially occluded text, etc.
  - **Link:** [CTW-download](https://ctwdataset.github.io/)

<a id="14-synthetic-datasets"></a>
### 1.4 Synthetic Datasets

* Synth90k [53] : 
  * **Introduction:** There are 9 million images of cropped word generated from a set of 90k common English words. Words are rendered onto natural images with random transformations and effects.
  * **Link:** [Synth90k-download](http://www.robots.ox.ac.uk/~vgg/data/text/)
* SynthText [54] : 
  * **Introduction:** There are 6 million images of cropped word. The generation process is similar to that of Synth90k.
  * **Link:** [SynthText-download](https://github.com/ankush-me/SynthText)

<a id="15-comparison-of-datasets"></a>
### 1.5 Comparison of Datasets

<table cellspacing="0" border="0">
	<colgroup width="156"></colgroup>
	<colgroup width="114"></colgroup>
	<colgroup width="121"></colgroup>
	<colgroup width="124"></colgroup>
	<colgroup width="152"></colgroup>
	<colgroup width="145"></colgroup>
	<colgroup width="135"></colgroup>
	<colgroup width="134"></colgroup>
	<colgroup span="6" width="84"></colgroup>
	<colgroup width="114"></colgroup>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" colspan=15 height="20" align="center"><b>Comparison of Datasets</b></td>
		</tr>
	<tr>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 height="39" align="center"><b>Datasets&emsp;&emsp;&emsp;&emsp;</b></td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b>Language&emsp;&emsp;&emsp;&emsp;</b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" colspan=6 align="center"><b>Images</b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" colspan=4 align="center"><b>Lexicon</b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" colspan=2 align="center"><b>Label</b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b>Types</b></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b>Pictures</b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b>Instances</b></td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b>Training Pictures</b></td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b>Training Instances</b></td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b>Testing Pictures</b></td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b>Testing Instances</b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="50" sdnum="2052;"><b><font face="Arial">50</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b><font face="Arial">1k</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b><font face="Arial">Full</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b><font face="Arial">None</font></b></td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b>Char</b></td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b>Word</b></td>
		</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">IIIT5K[31]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">English</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="5000" sdnum="2052;"><font face="Arial">5000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="5000" sdnum="2052;"><font face="Arial">5000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2000" sdnum="2052;"><font face="Arial">2000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2000" sdnum="2052;"><font face="Arial">2000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="3000" sdnum="2052;"><font face="Arial">3000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="3000" sdnum="2052;"><font face="Arial">3000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">regular</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">SVT[32]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">English</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="350" sdnum="2052;"><font face="Arial">350</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="100" sdnum="2052;"><font face="Arial">100</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="250" sdnum="2052;"><font face="Arial">250</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="647" sdnum="2052;"><font face="Arial">647</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">regular</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">IC03[33]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">English</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="509" sdnum="2052;"><font face="Arial">509</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="258" sdnum="2052;"><font face="Arial">258</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="251" sdnum="2052;"><font face="Arial">251</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="867" sdnum="2052;"><font face="Arial">867</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">regular</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">IC13[34]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">English</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="462" sdnum="2052;"><font face="Arial">462</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="229" sdnum="2052;"><font face="Arial">229</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="233" sdnum="2052;"><font face="Arial">233</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="1015" sdnum="2052;"><font face="Arial">1015</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">regular</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">SVHN[45]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">Digits</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="600000" sdnum="2052;"><font face="Arial">600000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="600000" sdnum="2052;"><font face="Arial">600000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="573968" sdnum="2052;"><font face="Arial">573968</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="573968" sdnum="2052;"><font face="Arial">573968</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="26032" sdnum="2052;"><font face="Arial">26032</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="26032" sdnum="2052;"><font face="Arial">26032</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">regular</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">SVT-P[35]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">English</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="238" sdnum="2052;"><font face="Arial">238</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="639" sdnum="2052;"><font face="Arial">639</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="238" sdnum="2052;"><font face="Arial">238</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="639" sdnum="2052;"><font face="Arial">639</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">irregular</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">CUTE80[36]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">English</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="80" sdnum="2052;"><font face="Arial">80</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="288" sdnum="2052;"><font face="Arial">288</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="80" sdnum="2052;"><font face="Arial">80</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="288" sdnum="2052;"><font face="Arial">288</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">irregular</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">IC15[37]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">English</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="1500" sdnum="2052;"><font face="Arial">1500</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="1000" sdnum="2052;"><font face="Arial">1000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="500" sdnum="2052;"><font face="Arial">500</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2077" sdnum="2052;"><font face="Arial">2077</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">irregular</font></td>
	</tr>
	<tr>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">COCO-Text[38]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">English</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="63686" sdnum="2052;"><font face="Arial">63686</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="145859" sdnum="2052;"><font face="Arial">145859</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="43686" sdnum="2052;"><font face="Arial">43686</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="118309" sdnum="2052;"><font face="Arial">118309</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2000" sdnum="2052;"><font face="Arial">2000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="27550" sdnum="2052;"><font face="Arial">27550</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">regular</font></td>
	</tr>
	<tr>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">Total-Text[39]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">English</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="1555" sdnum="2052;"><font face="Arial">1555</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="11459" sdnum="2052;"><font face="Arial">11459</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="1555" sdnum="2052;"><font face="Arial">1555</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="11459" sdnum="2052;"><font face="Arial">11459</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">irregular</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">CTW-1500[43]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">Chinese/English</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="1500" sdnum="2052;"><font face="Arial">1500</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="10751" sdnum="2052;"><font face="Arial">10751</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="1000" sdnum="2052;"><font face="Arial">1000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="500" sdnum="2052;"><font face="Arial">500</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">irregular</font></td>
	</tr>
	<tr>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">CTW-12K[40]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">Chinese</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="12514" sdnum="2052;"><font face="Arial">12514</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="11514" sdnum="2052;"><font face="Arial">11514</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="1000" sdnum="2052;"><font face="Arial">1000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">regular</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">MTWI[41]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">Chinese</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="20000" sdnum="2052;"><font face="Arial">20000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="10000" sdnum="2052;"><font face="Arial">10000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="10000" sdnum="2052;"><font face="Arial">10000</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">regular</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">CTW[42]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">Chinese</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="32285" sdnum="2052;"><font face="Arial">32285</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="1018402" sdnum="2052;"><font face="Arial">1018402</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="25887" sdnum="2052;"><font face="Arial">25887</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="812872" sdnum="2052;"><font face="Arial">812872</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="3269" sdnum="2052;"><font face="Arial">3269</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="103519" sdnum="2052;"><font face="Arial">103519</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">√</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">regular</font></td>
	</tr>
</table>

***

<a id="2-summary-of-scene-text-recognition-results"></a>
## 2. Summary of Scene Text Recognition Results

<a id="21-introduction"></a>
### 2.1 Introduction

As shown in Table "Summary of Scene Text Recognition Results", we summarize the main recognition algorithms in community from 2011 to the present. The content of the table includes the sources, highlights, codes, types and recognition performance. The '*' in the Method indicates the use of extra datasets. The **bold** in the numeric  represents the highest recognition results; ''^" represents the highest result of using the extra datasets; "@" represents different evaluation method which only uses 1811 test images. 

<a id="22-summary-of-scene-text-recognition-results"></a>
### 2.2 Summary of Scene Text Recognition Results

<table cellspacing="0" border="0">
	<colgroup width="271"></colgroup>
	<colgroup width="1051"></colgroup>
	<colgroup span="2" width="89"></colgroup>
	<colgroup width="106"></colgroup>
	<colgroup width="117"></colgroup>
	<colgroup span="13" width="89"></colgroup>
	<colgroup span="5" width="86"></colgroup>
	<colgroup width="103"></colgroup>
	<colgroup span="2" width="86"></colgroup>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" colspan=24 height="34" align="center"><b><font size=4>Summary of Scene Text Recognition Results</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><br></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><br></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><br></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 height="39" align="center"><b><font face="Arial">Method&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">Highlight&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">Code</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">Regular</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">Irregular</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">Segmentation</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">Extra data</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">CTC</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">Attention</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" colspan=3 align="center" bgcolor="#FFFFCC"><b><font face="Arial">IIIT5K</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" colspan=2 align="center" bgcolor="#FFFFCC"><b><font face="Arial">SVT</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" colspan=4 align="center" bgcolor="#FFFFCC"><b><font face="Arial">IC03</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC"><b><font face="Arial">IC13</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" colspan=3 align="center" bgcolor="#E6E6FF"><b><font face="Arial">SVT-P</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF"><b><font face="Arial">CUTE80</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF"><b><font face="Arial">IC15(2077)</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF"><b><font face="Arial">COCO-TEXT</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">Time</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">Source</font></b></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="50" sdnum="2052;"><b><font face="Arial">50</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC"><b><font face="Arial">1K</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC"><b><font face="Arial">None</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="50" sdnum="2052;"><b><font face="Arial">50</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC"><b><font face="Arial">None</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="50" sdnum="2052;"><b><font face="Arial">50</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC"><b><font face="Arial">Full</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC"><b><font face="Arial">50k</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC"><b><font face="Arial">None</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC"><b><font face="Arial">None</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="50" sdnum="2052;"><b><font face="Arial">50</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF"><b><font face="Arial">Full</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF"><b><font face="Arial">None</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF"><b><font face="Arial">None</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF"><b><font face="Arial">None</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF"><b><font face="Arial">None</font></b></td>
		</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">Wang et al. [1]: ABBYY</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors propose a two-stage text recognition system. The system consists of a state-of-the-art text detection followed by a leading OCR engine that shows outstanding performance.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000"> ×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="24.3" sdnum="2052;0;0.0"><font face="Arial">24.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="35" sdnum="2052;0;0.0"><font face="Arial">35.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="56" sdnum="2052;0;0.0"><font face="Arial">56.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="55" sdnum="2052;0;0.0"><font face="Arial">55.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="40.5" sdnum="2052;0;0.0"><font face="Arial">40.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="26.1" sdnum="2052;0;0.0"><font face="Arial">26.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2011" sdnum="2052;">2011</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ICCV</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Wang et al. [1] : SYNTH+PLEX</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors established a baseline for scene text recognition. The results showed that an object recognition-based pipeline outperform conventional OCR engines and do so without explicit use of a text detector, which significantly simplifying the recognition pipeline.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="57" sdnum="2052;0;0.0"><font face="Arial">57.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="76" sdnum="2052;0;0.0"><font face="Arial">76.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="62" sdnum="2052;0;0.0"><font face="Arial">62.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2011" sdnum="2052;">2011</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ICCV</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Mishra et al. [2]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors presented a new framework, which used CRF and some or all of the English dictionary as the priors to obtain the recognition results. Besides, they introduced the IIIT5K-word datasets.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="64.1" sdnum="2052;0;0.0"><font face="Arial">64.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="57.5" sdnum="2052;0;0.0"><font face="Arial">57.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="73.2" sdnum="2052;0;0.0"><font face="Arial">73.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="81.8" sdnum="2052;0;0.0"><font face="Arial">81.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="67.8" sdnum="2052;0;0.0"><font face="Arial">67.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="45.7" sdnum="2052;0;0.0"><font face="Arial">45.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="24.7" sdnum="2052;0;0.0"><font face="Arial">24.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2012" sdnum="2052;">2012</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">BMVC</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Wang et al. [3]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors built a new recognition system for scene text recognition task. They combined the representational power of multi-layer CNN, NMS and beam search in a end-to-end, lexicon-driven, scene text recognition system.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="70" sdnum="2052;0;0.0"><font face="Arial">70.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="90" sdnum="2052;0;0.0"><font face="Arial">90.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="84" sdnum="2052;0;0.0"><font face="Arial">84.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="40.2" sdnum="2052;0;0.0"><font face="Arial">40.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="32.4" sdnum="2052;0;0.0"><font face="Arial">32.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2012" sdnum="2052;">2012</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ICPR</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Goel et al. [4] : wDTW</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors presented a holistic word recognition framework which did not require explicit character segmentation. They generated synthetic images from lexicon words and recognized the text in the image by matching the scene and synthetic images features with wDTW.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="77.3" sdnum="2052;0;0.0"><font face="Arial">77.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="89.7" sdnum="2052;0;0.0"><font face="Arial">89.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2013" sdnum="2052;">2013</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ICDAR</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Bissacco et al. [5] : PhotoOCR</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors presented a two-stage text recognition system. The system was based on HOG features and recognized by a 5-layer CNN. Besides, they built a self-supervision mechanism to construct additional datasets.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="90.4" sdnum="2052;0;0.0"><font face="Arial">90.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="78" sdnum="2052;0;0.0"><font face="Arial">78.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="87.6" sdnum="2052;0;0.0"><font face="Arial">87.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2013" sdnum="2052;">2013</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ICCV</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Phan et al. [6]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed a two-stage text recognition system for scene text recognition with perspective distortion. The system used MSERs to detect characters, SIFT descriptors to extract features, and SVM clustering to recognize words. Besides, the SVT-P datasets was introduced.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="73.7" sdnum="2052;0;0.0"><font face="Arial">73.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="82.2" sdnum="2052;0;0.0"><font face="Arial">82.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="62.3" sdnum="2052;0;0.0"><font face="Arial">62.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="42.2" sdnum="2052;0;0.0"><font face="Arial">42.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2013" sdnum="2052;">2013</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ICCV</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Alsharif et al. [7] : HMM/Maxout</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">Authors constructed a two-stage text recognition system based on segmentation method. The system recognized words by leveraging the convolutional Maxout networks along with hybrid HMM models. Besides, author showed the performance of end-to-end recognition.</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="74.3" sdnum="2052;0;0.0"><font face="Arial">74.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.1" sdnum="2052;0;0.0"><font face="Arial">93.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="88.6" sdnum="2052;0;0.0"><font face="Arial">88.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="85.1" sdnum="2052;0;0.0"><font face="Arial">85.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2014" sdnum="2052;">2014</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ICLR</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Almazan et al [8] : KCSR</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors embedded the word images and text strings in a common vectorial subspace, and regarded the recognition task as a nearest neighbor problem. The proposed representation had a fixed length, low dimensional and was fast to compute.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="88.6" sdnum="2052;0;0.0"><font face="Arial">88.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="75.6" sdnum="2052;0;0.0"><font face="Arial">75.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="87" sdnum="2052;0;0.0"><font face="Arial">87.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2014" sdnum="2052;">2014</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">TPAMI</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Yao et al. [9] : Strokelets</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">Authors proposed a novel multi-scale representation 'Strokelets' for scene text recognition. Strokelets possed four distinctive advantages: usability, robustness, generality and expressivity.</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">×</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="80.2" sdnum="2052;0;0.0"><font face="Arial">80.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="69.3" sdnum="2052;0;0.0"><font face="Arial">69.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="75.9" sdnum="2052;0;0.0"><font face="Arial">75.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="88.5" sdnum="2052;0;0.0"><font face="Arial">88.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="80.3" sdnum="2052;0;0.0"><font face="Arial">80.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2014" sdnum="2052;">2014</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">CVPR</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">R.-Serrano et al.[10] : Label embedding</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors embedded word labels and word images into a common Euclidean space. The advantages of proposed method was simple and effective. It could combine with any descriptor and did not require costly pre-/post-processing operations.  It also allowed for the recognition of never-seen before words.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="76.1" sdnum="2052;0;0.0"><font face="Arial">76.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="57.4" sdnum="2052;0;0.0"><font face="Arial">57.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="70" sdnum="2052;0;0.0"><font face="Arial">70.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2015" sdnum="2052;">2015</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">IJCV</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Jaderberg et al. [11]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed a novel CNN classifier that enabled efficient feature sharing for text detection, character case-sensitive and insensitive classification, and bi-gram classification. Besides, they proposed a method of automated data mining of Flickr.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="86.1" sdnum="2052;0;0.0"><font face="Arial">86.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.2" sdnum="2052;0;0.0"><font face="Arial">96.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="91.5" sdnum="2052;0;0.0"><font face="Arial">91.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2014" sdnum="2052;">2014</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ECCV</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Su and Lu [12]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed a novel method that recognized the whole word images without character-level segmentation. The proposed method was based on HOG features, using BLSTM and CTC to achieve text recognition.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="83" sdnum="2052;0;0.0"><font face="Arial">83.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="92" sdnum="2052;0;0.0"><font face="Arial">92.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="82" sdnum="2052;0;0.0"><font face="Arial">82.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2014" sdnum="2052;">2014</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ACCV</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Gordo[13] : Mid-features</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed a descriptive, robust, and compact fixed-length representation: mid-level features. The proposed features could be paired with word attributes framework to improve recognition performance.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.3" sdnum="2052;0;0.0"><font face="Arial">93.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="86.6" sdnum="2052;0;0.0"><font face="Arial">86.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="91.8" sdnum="2052;0;0.0"><font face="Arial">91.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2015" sdnum="2052;">2015</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">CVPR</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Jaderberg et al. [14]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors presented an end-to-end system for text localizing and recognizing in natural scene images and a synthetic dataset containing 9 million images. The proposed system used CNN to identify text, and the categories was 90k, which covered almost all words. Besides, the recognition result of the system can be used to update the detector.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.1" sdnum="2052;0;0.0"><font face="Arial">97.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="92.7" sdnum="2052;0;0.0"><font face="Arial">92.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95.4" sdnum="2052;0;0.0"><font face="Arial">95.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="80.7" sdnum="2052;0;0.0"><font face="Arial">80.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.7" sdnum="2052;0;0.0"><font face="Arial">98.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.6" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF3333">98.6</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.3" sdnum="2052;0;0.0"><font face="Arial">93.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.1" sdnum="2052;0;0.0"><font face="Arial">93.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="90.8" sdnum="2052;0;0.0"><font face="Arial">90.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2015" sdnum="2052;">2015</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">IJCV</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Jaderberg et al. [15]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed a model incorporating CNN and CRF for the unconstrained recognition of words in natural images. The entire model could be jointly optimized by back-propagating the structured output loss. The results set the baseline for lexicon-free.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95.5" sdnum="2052;0;0.0"><font face="Arial">95.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="89.6" sdnum="2052;0;0.0"><font face="Arial">89.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.2" sdnum="2052;0;0.0"><font face="Arial">93.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="71.7" sdnum="2052;0;0.0"><font face="Arial">71.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.8" sdnum="2052;0;0.0"><font face="Arial">97.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97" sdnum="2052;0;0.0"><font face="Arial">97.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.4" sdnum="2052;0;0.0"><font face="Arial">93.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="89.6" sdnum="2052;0;0.0"><font face="Arial">89.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="81.8" sdnum="2052;0;0.0"><font face="Arial">81.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2015" sdnum="2052;">2015</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ICLR</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Shi, Bai, and Yao [16] : CRNN</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors modeled scene text recognition as a sequence problem by integrating the advantages of both deep CNN and RNN. They proposed an end-to-end trainable framework where transcription was made by CTC.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.8" sdnum="2052;0;0.0"><font face="Arial">97.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95" sdnum="2052;0;0.0"><font face="Arial">^95.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="81.2" sdnum="2052;0;0.0"><font face="Arial">81.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.5" sdnum="2052;0;0.0"><font face="Arial">97.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="82.7" sdnum="2052;0;0.0"><font face="Arial">82.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.7" sdnum="2052;0;0.0"><font face="Arial">98.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98" sdnum="2052;0;0.0"><font face="Arial">98.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95.7" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF3333">95.7</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="91.9" sdnum="2052;0;0.0"><font face="Arial">91.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="89.6" sdnum="2052;0;0.0"><font face="Arial">89.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2017" sdnum="2052;">2017</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">TPAMI</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Shi et al. [17] : RARE</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed RARE, a recognition model for irregular text. The input images were firstly rectified via STN, extracted features by CNN, and then decoded by a recurrent network based on attention mechanism.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.2" sdnum="2052;0;0.0"><font face="Arial">96.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.8" sdnum="2052;0;0.0"><font face="Arial">93.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="81.9" sdnum="2052;0;0.0"><font face="Arial">81.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95.5" sdnum="2052;0;0.0"><font face="Arial">95.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="81.9" sdnum="2052;0;0.0"><font face="Arial">81.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.3" sdnum="2052;0;0.0"><font face="Arial">98.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.2" sdnum="2052;0;0.0"><font face="Arial">96.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94.8" sdnum="2052;0;0.0"><font face="Arial">94.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="90.1" sdnum="2052;0;0.0"><font face="Arial">90.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="88.6" sdnum="2052;0;0.0"><font face="Arial">88.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="91.2" sdnum="2052;0;0.0"><font face="Arial">91.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="77.4" sdnum="2052;0;0.0"><font face="Arial">77.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="71.8" sdnum="2052;0;0.0"><font face="Arial">71.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="59.2" sdnum="2052;0;0.0"><font face="Arial">59.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2016" sdnum="2052;">2016</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">CVPR</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Lee and Osindero [18] : R2AM</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed recursive CNN, which allowed for parametrically efficient and effective image feature extraction. They constructed R2AM, which implicitly learned character-level language model. The use of a soft-attention mechanism allowed the model to decode selectively. </font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.8" sdnum="2052;0;0.0"><font face="Arial">96.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94.4" sdnum="2052;0;0.0"><font face="Arial">94.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="78.4" sdnum="2052;0;0.0"><font face="Arial">78.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.3" sdnum="2052;0;0.0"><font face="Arial">96.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="80.7" sdnum="2052;0;0.0"><font face="Arial">80.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.9" sdnum="2052;0;0.0"><font face="Arial">97.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97" sdnum="2052;0;0.0"><font face="Arial">97.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="88.7" sdnum="2052;0;0.0"><font face="Arial">88.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="90" sdnum="2052;0;0.0"><font face="Arial">90.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2016" sdnum="2052;">2016</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">CVPR</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">Liu et al.  [19] : STAR-Net</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors presented the STAR-Net for irregular scene text recognition. The proposed network used STN to remove the distortions of texts, which reduced the difficulty of recognition module. The residue convolutional blocks were employed for extracting image-based features, and words were decoded by BLSTM and CTC.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.7" sdnum="2052;0;0.0"><font face="Arial">97.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94.5" sdnum="2052;0;0.0"><font face="Arial">94.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="83.3" sdnum="2052;0;0.0"><font face="Arial">83.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95.5" sdnum="2052;0;0.0"><font face="Arial">95.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="83.6" sdnum="2052;0;0.0"><font face="Arial">83.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.9" sdnum="2052;0;0.0"><font face="Arial">96.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95.3" sdnum="2052;0;0.0"><font face="Arial">95.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="89.9" sdnum="2052;0;0.0"><font face="Arial">89.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="89.1" sdnum="2052;0;0.0"><font face="Arial">89.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="94.3" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF0000">94.3</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="83.6" sdnum="2052;0;0.0"><font face="Arial">83.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="73.5" sdnum="2052;0;0.0"><font face="Arial">73.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2016" sdnum="2052;">2016</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">BMVC</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">*Yang et al. [20]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors presented a robust end-to-end neural-based model to attentively recognize text in natural images. An auxiliary dense character detection task was introduced that helped to learn text specific visual patterns. A recurrent decoder  network based on the attention mechanism that generated target sequences. Besides, they proposed a synthetic dataset containing perspective distortion, curvature, etc.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.8" sdnum="2052;0;0.0"><font face="Arial">97.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.1" sdnum="2052;0;0.0"><font face="Arial">96.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95.2" sdnum="2052;0;0.0"><font face="Arial">95.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.7" sdnum="2052;0;0.0"><font face="Arial">97.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="93" sdnum="2052;0;0.0"><font face="Arial">93.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="80.2" sdnum="2052;0;0.0"><font face="Arial">80.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="75.8" sdnum="2052;0;0.0"><font face="Arial">75.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="69.3" sdnum="2052;0;0.0"><font face="Arial">69.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2017" sdnum="2052;">2017</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">IJCAI</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">Yin et al. [21]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed a novel system for scene text recognition. The method simultaneously detected and recognized characters by sliding the text line image with character
models. CNN was used to extract image-based feature and the final recognition results were decoded with CTC based algorithm.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.7" sdnum="2052;0;0.0"><font face="Arial">98.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.1" sdnum="2052;0;0.0"><font face="Arial">96.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="78.2" sdnum="2052;0;0.0"><font face="Arial">78.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95.1" sdnum="2052;0;0.0"><font face="Arial">95.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="72.5" sdnum="2052;0;0.0"><font face="Arial">72.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.6" sdnum="2052;0;0.0"><font face="Arial">97.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.5" sdnum="2052;0;0.0"><font face="Arial">96.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="81.1" sdnum="2052;0;0.0"><font face="Arial">81.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="81.4" sdnum="2052;0;0.0"><font face="Arial">81.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2017" sdnum="2052;">2017</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ICCV</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">*Cheng et al. [22] : FAN</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed the concept of 'attention drift' and  a novel method called FAN for scene text recognition. A focusing network (FN) was introduced, which
could focus AN’s deviated attention back on the target areas.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="99.3" sdnum="2052;0;0.0"><font face="Arial">99.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.5" sdnum="2052;0;0.0"><font face="Arial">97.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="87.4" sdnum="2052;0;0.0"><font face="Arial">87.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.1" sdnum="2052;0;0.0"><font face="Arial">97.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="85.9" sdnum="2052;0;0.0"><font face="Arial">85.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="99.2" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF3333">99.2</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.3" sdnum="2052;0;0.0"><font face="Arial">97.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94.2" sdnum="2052;0;0.0"><font face="Arial">94.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.3" sdnum="2052;0;0.0"><font face="Arial">93.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><b><font face="Arial" color="#339966">@85.3</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2017" sdnum="2052;">2017</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ICCV</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">Cheng et al. [23] : AON</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors developed the arbitrary orientation network (AON) to directly capture the
deep features of irregular texts. The proposed network extracted scene text features in four directions and the character placement clues. A filter gate (FG) was designed for fusing four-direction features with the learned placement clues.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="99.6" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF0000">99.6</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.1" sdnum="2052;0;0.0"><font face="Arial">98.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="87" sdnum="2052;0;0.0"><font face="Arial">87.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96" sdnum="2052;0;0.0"><font face="Arial">96.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="82.8" sdnum="2052;0;0.0"><font face="Arial">82.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.5" sdnum="2052;0;0.0"><font face="Arial">98.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.1" sdnum="2052;0;0.0"><font face="Arial">97.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="91.5" sdnum="2052;0;0.0"><font face="Arial">91.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="94" sdnum="2052;0;0.0"><font face="Arial">94.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="83.7" sdnum="2052;0;0.0"><font face="Arial">83.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="73" sdnum="2052;0;0.0"><font face="Arial">73.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="76.8" sdnum="2052;0;0.0"><font face="Arial">76.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="68.2" sdnum="2052;0;0.0"><font face="Arial">68.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2018" sdnum="2052;">2018</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">CVPR</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Gao et al. [24]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed a novel scene text recognition system. In order to suppress the background noise, the residual attention modules were incorporated into a small densely connected network to improve the discriminability of CNN features. Besides, the proposed system speed up recognition by removing the RNN.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="99.1" sdnum="2052;0;0.0"><font face="Arial" color="#000000">99.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.9" sdnum="2052;0;0.0"><font face="Arial">97.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="81.8" sdnum="2052;0;0.0"><font face="Arial">81.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.4" sdnum="2052;0;0.0"><font face="Arial">97.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="82.7" sdnum="2052;0;0.0"><font face="Arial">82.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.7" sdnum="2052;0;0.0"><font face="Arial">98.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.7" sdnum="2052;0;0.0"><font face="Arial">96.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="89.2" sdnum="2052;0;0.0"><font face="Arial">89.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="88" sdnum="2052;0;0.0"><font face="Arial">88.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2017" sdnum="2052;">2017</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">arXiv</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Liu et al.  [25] : Char-Net</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors presented a Char-Net for recognizing distorted scene text. The proposed system extracted the single-character feature region and removed distortion of it. Finally, the recurrent decoder network based on the attention mechanism generated target sequences.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="83.6" sdnum="2052;0;0.0"><font face="Arial">83.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="84.4" sdnum="2052;0;0.0"><font face="Arial">84.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.3" sdnum="2052;0;0.0"><font face="Arial">93.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="91.5" sdnum="2052;0;0.0"><font face="Arial">91.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="90.8" sdnum="2052;0;0.0"><font face="Arial">90.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="73.5" sdnum="2052;0;0.0"><font face="Arial">73.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="60" sdnum="2052;0;0.0"><font face="Arial">60.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2018" sdnum="2052;">2018</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">AAAI</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">*Liu et al.  [26] : SqueezedText</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed SqueezedText for real-time scene text recognition. The front-end B-CEDNet was trained under binary constraints with significant compression . Hence, the proposed method lead to both remarkable inference run-time speedup as well as memory usage reduction.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97" sdnum="2052;0;0.0"><font face="Arial">97.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94.1" sdnum="2052;0;0.0"><font face="Arial">94.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="87" sdnum="2052;0;0.0"><font face="Arial">87.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95.2" sdnum="2052;0;0.0"><font face="Arial">95.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.8" sdnum="2052;0;0.0"><font face="Arial">98.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.9" sdnum="2052;0;0.0"><font face="Arial">97.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.8" sdnum="2052;0;0.0"><font face="Arial">93.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.1" sdnum="2052;0;0.0"><font face="Arial">93.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="92.9" sdnum="2052;0;0.0"><font face="Arial">92.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2018" sdnum="2052;">2018</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">AAAI</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">*Bai et al. [27] : EP</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors focused on the the misalignment between the ground truth strings and the attention’s output sequences of probability distribution and proposed EP for scene text recognition. The advantage of using edit probability was that the training process could focus on the missing, superfluous and unrecognized characters, and thus the impact of the misalignment
problem could be alleviated or even overcome.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="99.5" sdnum="2052;0;0.0"><font face="Arial">99.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.9" sdnum="2052;0;0.0"><font face="Arial">97.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="88.3" sdnum="2052;0;0.0"><font face="Arial">88.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.6" sdnum="2052;0;0.0"><font face="Arial">96.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="87.5" sdnum="2052;0;0.0"><font face="Arial">87.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.7" sdnum="2052;0;0.0"><font face="Arial">98.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.9" sdnum="2052;0;0.0"><font face="Arial">97.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94.6" sdnum="2052;0;0.0"><font face="Arial">94.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94.4" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">^94.4</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="73.9" sdnum="2052;0;0.0"><font face="Arial">73.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2018" sdnum="2052;">2018</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">CVPR</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Liu et al. [28]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors addressed the problem of image feature learning for scene text recognition. The novel multi-task network was presented with an encoder-generator-discriminator-decoder architecture that guided image feature learning by using clean images.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.3" sdnum="2052;0;0.0"><font face="Arial">97.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.1" sdnum="2052;0;0.0"><font face="Arial">96.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="89.4" sdnum="2052;0;0.0"><font face="Arial">89.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.8" sdnum="2052;0;0.0"><font face="Arial">96.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="87.1" sdnum="2052;0;0.0"><font face="Arial">87.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.1" sdnum="2052;0;0.0"><font face="Arial">98.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.5" sdnum="2052;0;0.0"><font face="Arial">97.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94.7" sdnum="2052;0;0.0"><font face="Arial" color="#000000">94.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94" sdnum="2052;0;0.0"><font face="Arial">94.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="73.9" sdnum="2052;0;0.0"><font face="Arial">73.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="62.5" sdnum="2052;0;0.0"><font face="Arial">62.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2018" sdnum="2052;">2018</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ECCV</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">Gao et al. [29]</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed a novel scene text recognition system. In order to suppress the background noise, the residual attention modules were incorporated into a small densely connected network to improve the discriminability of CNN features. Finally, a recurrent decoder based on CTC algorithm generated the recognition results.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="99.1" sdnum="2052;0;0.0"><font face="Arial">99.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.2" sdnum="2052;0;0.0"><font face="Arial">97.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="83.6" sdnum="2052;0;0.0"><font face="Arial">83.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.7" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF0000">97.7</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="83.9" sdnum="2052;0;0.0"><font face="Arial">83.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.6" sdnum="2052;0;0.0"><font face="Arial">98.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.6" sdnum="2052;0;0.0"><font face="Arial">96.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="91.4" sdnum="2052;0;0.0"><font face="Arial" color="#000000">91.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="89.5" sdnum="2052;0;0.0"><font face="Arial">89.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2018" sdnum="2052;">2018</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ICIP</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">Shi et al. [30] : ASTER</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed ASTER for irregular scene text recognition. The proposed system was an improved version of [17]. The input images were firstly rectified via TPS, extracted features by Res-Net, and then decoded by a recurrent network based on attention mechanism.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="99.6" sdnum="2052;0;0.0"><font face="Arial">99.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.8" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF0000">98.8</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="93.4" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF0000">93.4</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.4" sdnum="2052;0;0.0"><font face="Arial" color="#000000">97.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="89.5" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF0000">89.5</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.8" sdnum="2052;0;0.0"><font face="Arial">98.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98" sdnum="2052;0;0.0"><font face="Arial">98.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94.5" sdnum="2052;0;0.0"><font face="Arial">94.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="91.8" sdnum="2052;0;0.0"><font face="Arial">91.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="78.5" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF0000">78.5</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="79.5" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF0000">79.5</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="76.1" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF0000">76.1</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2018" sdnum="2052;">2018</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">TPAMI</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">Luo et al. [46] : MORAN</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors designed MORAN for rectifying images that contain irregular text. The proposed method predicted the offsets of different regions in text images, decreased the difficulty of recognition and enabled the attention-based sequence recognition network to more easily read irregular text. Compared with TPS, MORAN was simpler and more usable.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.9" sdnum="2052;0;0.0"><font face="Arial" color="#000000">97.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.2" sdnum="2052;0;0.0"><font face="Arial" color="#000000">96.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="91.2" sdnum="2052;0;0.0"><font face="Arial" color="#000000">91.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.6" sdnum="2052;0;0.0"><font face="Arial" color="#000000">96.6</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="88.3" sdnum="2052;0;0.0"><font face="Arial" color="#000000">88.3</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.7" sdnum="2052;0;0.0"><font face="Arial" color="#000000">98.7</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.8" sdnum="2052;0;0.0"><font face="Arial">97.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF3333">95.0</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="92.4" sdnum="2052;0;0.0"><font face="Arial">92.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="94.3" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF0000">94.3</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="86.7" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF0000">86.7</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="76.1" sdnum="2052;0;0.0"><font face="Arial">76.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="77.4" sdnum="2052;0;0.0"><font face="Arial">77.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="68.8" sdnum="2052;0;0.0"><font face="Arial">68.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2019" sdnum="2052;">2019</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">PR</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="46" align="center"><font face="Arial">Xie et al. [47] : CAN</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors presented CAN for unconstrained scene text recognition. A Res-Net was used to extract image-based features .CNN and GLU were incorporated as the decoder instead of RNN to obtain the final recognition result.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97" sdnum="2052;0;0.0"><font face="Arial" color="#000000">97.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94.2" sdnum="2052;0;0.0"><font face="Arial" color="#000000">94.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="80.5" sdnum="2052;0;0.0"><font face="Arial" color="#000000">80.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="96.9" sdnum="2052;0;0.0"><font face="Arial" color="#000000">96.9</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="83.4" sdnum="2052;0;0.0"><font face="Arial" color="#000000">83.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.4" sdnum="2052;0;0.0"><font face="Arial" color="#000000">98.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="97.8" sdnum="2052;0;0.0"><font face="Arial" color="#000000">97.8</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="91" sdnum="2052;0;0.0"><font face="Arial" color="#000000">91.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="90.5" sdnum="2052;0;0.0"><font face="Arial" color="#000000">90.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2019" sdnum="2052;">2019</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">ACM</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">*Liao et al.[48] : CA-FCN</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">CA-FCN was devised for recognizing the text of arbitrary shapes. The proposed method was conducted from two-dimensional perspective and could simultaneously recognize the script and predict the position of each character. Besides, the proposed method required character-level labeling.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="99.8" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">^99.8</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.9" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">^98.9</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="92" sdnum="2052;0;0.0"><font face="Arial">92.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.8" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">^98.8</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="82.1" sdnum="2052;0;0.0"><font face="Arial" color="#000000">82.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="91.4" sdnum="2052;0;0.0"><font face="Arial">91.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="78.1" sdnum="2052;0;0.0"><font face="Arial">78.1</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2019" sdnum="2052;">2019</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">AAAI</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="47" align="center"><font face="Arial">*Li et al. [49] : SAR</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">Authors proposed SAR for irregular scene text recognition. A Res-Net was used to extract image features and the decoder network based on the 2D-attention mechanism generated target sequences.</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial" color="#000000">×</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font color="#000000">√</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="99.4" sdnum="2052;0;0.0"><font face="Arial">99.4</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.2" sdnum="2052;0;0.0"><font face="Arial">98.2</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="95" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">95.0</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="98.5" sdnum="2052;0;0.0"><font face="Arial" color="#000000">98.5</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="91.2" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">^91.2</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#FFFFCC" sdval="94" sdnum="2052;0;0.0"><font face="Arial">94.0</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="95.8" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">^95.8</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="91.2" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">^91.2</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="86.4" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">^86.4</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="89.6" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">^89.6</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdval="78.8" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">^78.8</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" bgcolor="#E6E6FF" sdnum="2052;0;0.0"><b><font face="Arial" color="#FF6666">^66.8</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2019" sdnum="2052;">2019</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><font face="Arial">AAAI</font></td>
	</tr>
</table>



<a id="23-chinese-scene-text-recognition-results"></a>
### 2.3 Chinese Scene Text Recognition Results

<table cellspacing="0" border="0">
	<colgroup width="356"></colgroup>
	<colgroup width="112"></colgroup>
	<colgroup width="107"></colgroup>
	<colgroup width="103"></colgroup>
	<colgroup span="2" width="86"></colgroup>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" colspan=6 height="34" align="center"><b><font size=4>Chinese Scene Text Recognition Results</font></b></td>
		</tr>
	<tr>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 height="39" align="center"><b><font face="Arial">Method</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">RCTW</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">MTWI</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">CTW</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">Time</font></b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" rowspan=2 align="center"><b><font face="Arial">Source</font></b></td>
	</tr>
	<tr>
		</tr>
	<tr>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="23" align="center">Zheqi He,Yongtao Wang : Foo &amp; Bar</td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b>82.0 (end-to-end)</b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2017" sdnum="2052;">2017</td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">RCTW competition</td>
	</tr>
	<tr>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="25" align="center"><font face="Arial">IFLYTEK : nelslip(iflytek&amp;ustc)</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b>85.8 (AR)</b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2018" sdnum="2052;">2018</td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">MTWI competition</td>
	</tr>
	<tr>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">Yuan et al.[42] : CTW</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center"><b>80.5 (AR)</b></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2018" sdnum="2052;">2018</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">CTW</td>
	</tr>
	<tr>
		<td style="text-overflow:ellipsis;word-break:keep-all; white-space:nowrap;border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="center"><font face="Arial">Liu et al. [43] : CTW-1500</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdnum="2052;0;0.0"><font face="Arial">-</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center" sdval="2017" sdnum="2052;">2017</td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="center">CTW-1500</td>
	</tr>
</table>

***

<a id="3-field-survey"></a>
## 3. Field Survey

**[50] \[TPAMI-2015]** Ye Q, Doermann D. Text detection and recognition in imagery: A survey[J]. IEEE transactions on pattern analysis and machine intelligence, 2015, 37(7): 1480-1500. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6945320)

**[51] \[Frontiers-Comput. Sci-2016]** Zhu Y, Yao C, Bai X. Scene text detection and recognition: Recent advances and future trends[J]. Frontiers of Computer Science, 2016, 10(1): 19-36. [paper](https://link.springer.com/article/10.1007/s11704-015-4488-0)

**[52] \[arXiv-2018]** Long S, He X, Ya C. Scene Text Detection and Recognition: The Deep Learning Era[J]. arXiv preprint arXiv:1811.04256, 2018. [paper](https://arxiv.org/pdf/1811.04256.pdf)

***

<a id="4-ocr-service"></a>
## 4. OCR Service

|                             OCR                              | API  | Free |
| :----------------------------------------------------------: | :--: | :--: |
| [Tesseract OCR Engine](https://github.com/tesseract-ocr/tesseract) |  ×   |  √   |
| [Azure](https://azure.microsoft.com/zh-cn/services/cognitive-services/computer-vision/#Analysis) |  √   |  √   |
| [ABBYY](https://www.abbyy.cn/real-time-recognition-sdk/technical-specifications/) |  √   |  √   |
|               [OCR Space](https://ocr.space/)                |  √   |  √   |
|       [SODA PDF OCR](https://www.sodapdf.com/ocr-pdf/)       |  √   |  √   |
|          [Free Online OCR](https://www.newocr.com/)          |  √   |  √   |
|           [Online OCR](https://www.onlineocr.net/)           |  √   |  √   |
|             [Super Tools](https://www.wdku.net/)             |  √   |  √   |
|          [在线中文识别](http://chongdata.com/ocr/)           |  √   |  √   |
|   [Calamari OCR](https://github.com/Calamari-OCR/calamari)   |  ×   |  √   |
|   [腾讯OCR](https://cloud.tencent.com/product/ocr?lang=cn)   |  √   |  ×   |

***

<a id="5-references"></a>
## 5. References

**[1] \[ICCV-2011]** K. Wang, B. Babenko, and S. Belongie. End-to-end scene text recognition. In Proceedings of International Conference on Computer Vision (ICCV), pages 1457–1464, 2011. [paper ](https://www.researchgate.net/profile/Serge_Belongie/publication/221110077_End-to-end_scene_text_recognition/links/09e4150b34908d2ebb000000/End-to-end-scene-text-recognition.pdf)

**[2] \[BMVC-2012]** A. Mishra, K. Alahari, and C. Jawahar. Scene text recognition using higher order language priors. In Proceedings of British Machine Vision Conference (BMVC), pages 1–11, 2012. [paper](https://hal.inria.fr/hal-00818183/document) [dataset](http://cvit.iiit.ac.in/research/projects/cvit-projects/the-iiit-5k-word-dataset)

**[3] \[ICPR-2012]** T. Wang, D. J. Wu, A. Coates, and A. Y. Ng. End-to-end text recognition with convolutional neural networks. In Proceedings of International Conference on Pattern Recognition (ICPR), pages 3304–3308, 2012. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6460871&tag=1)

**[4] \[ICDAR-2013]** V. Goel, A. Mishra, K. Alahari, and C. Jawahar. Whole is greater than sum of parts: Recognizing scene text words. In Proceedings of International Conference on Document Analysis and Recognition (ICDAR), pages 398–402, 2013. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6628652) 

**[5] \[ICCV-2013]** A. Bissacco, M. Cummins, Y. Netzer, and H. Neven. Photoocr: Reading text in uncontrolled conditions. In Proceedings of International Conference on Computer Vision (ICCV), pages 785–792, 2013. [paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Bissacco_PhotoOCR_Reading_Text_2013_ICCV_paper.pdf)

**[6] \[ICCV-2013]** T. Quy Phan, P. Shivakumara, S. Tian, and C. Lim Tan. Recognizing text with perspective distortion in natural scenes.In Proceedings of International Conference on Computer Vision (ICCV), pages 569–576, 2013. [paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Phan_Recognizing_Text_with_2013_ICCV_paper.pdf)

**[7] \[ICLR-2014]** O. Alsharif and J. Pineau, End-to-end text recognition with hybrid HMM maxout models, in: Proceedings of International Conference on Learning Representations (ICLR), 2014. [paper](https://arxiv.org/pdf/1310.1811.pdf)

**[8] \[TPAMI-2014]** J. Almaz ́ an, A. Gordo, A. Forn ́ es, and E. Valveny. Word spotting and recognition with embedded attributes. IEEE Trans.Pattern Anal. Mach. Intell ., 36(12):2552–2566, 2014. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6857995) [code](https://github.com/almazan/watts)

**[9] \[CVPR-2014]** C. Yao, X. Bai, B. Shi, and W. Liu. Strokelets: A learned multi-scale representation for scene text recognition. In Proceedings of Computer Vision and Pattern Recognition (CVPR), pages 4042–4049, 2014. [paper](http://openaccess.thecvf.com/content_cvpr_2014/papers/Yao_Strokelets_A_Learned_2014_CVPR_paper.pdf)

**[10] \[IJCV-2015]** J. A. Rodriguez-Serrano, A. Gordo, and F. Perronnin. Label embedding: A frugal baseline for text recognition. International Journal of Computer Vision (IJCV) , 113(3):193–207, 2015. [paper](https://link.springer.com/content/pdf/10.1007%2Fs11263-014-0793-6.pdf)

**[11] \[ECCV-2014]** M. Jaderberg, A. Vedaldi, and A. Zisserman. Deep features for text spotting. In Proceedings of European Conference on Computer Vision (ECCV), pages 512–528, 2014. [paper](https://link.springer.com/content/pdf/10.1007%2F978-3-319-10593-2_34.pdf) [code](https://bitbucket.org/jaderberg/eccv2014_textspotting/src/master/)

**[12] \[ACCV-2014]** B. Su and S. Lu. Accurate scene text recognition based on recurrent neural network. In Proceedings of Asian Conference on Computer Vision (ACCV), pages 35–48, 2014. [paper](https://link.springer.com/content/pdf/10.1007%2F978-3-319-16865-4_3.pdf)

**[13] \[CVPR-2015]** A. Gordo. Supervised mid-level features for word image representation. In Proceedings of Computer Vision and Pattern Recognition (CVPR), pages 2956–2964, 2015. [paper](http://openaccess.thecvf.com/content_cvpr_2015/papers/Gordo_Supervised_Mid-Level_Features_2015_CVPR_paper.pdf)

**[14] \[IJCV-2015]** M. Jaderberg, K. Simonyan, A. Vedaldi, and A. Zisserman. Reading text in the wild with convolutional neural networks. Int. J.Comput. Vision, 2015. [paper](https://link.springer.com/content/pdf/10.1007%2Fs11263-015-0823-z.pdf) [code](http://www.robots.ox.ac.uk/~vgg/research/text/)

**[15] \[ICLR-2015]** M. Jaderberg, K. Simonyan, A. Vedaldi, A. Zisserman, Deep structured output learning for unconstrained text recognition, in: Proceedings of International Conference on Learning Representations (ICLR), 2015. [paper](https://arxiv.org/pdf/1412.5903.pdf)

**[16] \[TPAMI-2017]** B. Shi, X. Bai, and C. Yao. An end-to-end trainable neural network for image-based sequence recognition and its application to scene text recognition. IEEE Trans. Pattern Anal. Mach. Intell., 39(11):2298–2304, 2017. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7801919) [code-Torch7](https://github.com/bgshih/crnn) [code-Pytorch](https://github.com/meijieru/crnn.pytorch)

**[17] \[CVPR-2016]** B. Shi, X. Wang, P. Lyu, C. Yao, and X. Bai. Robust scene text recognition with automatic rectification. In Proceedings of Computer Vision and Pattern Recognition (CVPR), pages 4168–4176, 2016. [paper](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Shi_Robust_Scene_Text_CVPR_2016_paper.pdf)

**[18] \[CVPR-2016]** C.-Y. Lee and S. Osindero. Recursive recurrent nets with attention modeling for OCR in the wild. In Proceedings of Computer Vision and Pattern Recognition (CVPR), pages 2231–2239, 2016. [paper](http://openaccess.thecvf.com/content_cvpr_2016/papers/Lee_Recursive_Recurrent_Nets_CVPR_2016_paper.pdf)

**[19] \[BMVC-2016]** W. Liu, C. Chen, K.-Y. K. Wong, Z. Su, and J. Han. STAR-Net: A spatial attention residue network for scene text recognition. In Proceedings of British Machine Vision Conference (BMVC), page 7, 2016. [paper](https://i.cs.hku.hk/~kykwong/publications/wliu_bmvc16.pdf)

**[20] \[IJCAI-2017]** X. Yang, D. He, Z. Zhou, D. Kifer, and C. L. Giles. Learning to read irregular text with attention mechanisms. Proceedings of International Joint Conference on Artificial Intelligence (IJCAI), 2017. [paper](https://pdfs.semanticscholar.org/1259/f7533abe2fe85fd9dead92853e2ff07a8792.pdf)

**[21] \[ICCV-2017]** F. Yin, Y.-C. Wu, X.-Y. Zhang, and C.-L. Liu. Scene text recognition with sliding convolutional character models. In Proceedings of International Conference on Computer Vision (ICCV), 2017. [paper](https://arxiv.org/pdf/1709.01727.pdf)

**[22] \[ICCV-2017]** Z. Cheng, F. Bai, Y. Xu, G. Zheng, S. Pu, and S. Zhou. Focusing attention: Towards accurate text recognition in natural images. In Proceedings of International Conference on Computer Vision (ICCV), pages 5086–5094, 2017. [paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Cheng_Focusing_Attention_Towards_ICCV_2017_paper.pdf)

**[23] \[CVPR-2018]** Cheng Z, Xu Y, Bai F, et al. AON: Towards Arbitrarily-Oriented Text Recognition.In Proceedings of Computer Vision and Pattern Recognition (CVPR), pages 5571-5579, 2018. [paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Cheng_AON_Towards_Arbitrarily-Oriented_CVPR_2018_paper.pdf)

**[24] \[arXiv-2017]** Gao Y, Chen Y, Wang J, et al. Reading Scene Text with Attention Convolutional Sequence Modeling[J]. arXiv preprint arXiv:1709.04303, 2017. [paper](https://arxiv.org/pdf/1709.04303.pdf)

**[25] \[AAAI-2018]** Liu W, Chen C, Wong K Y K. Char-Net: A Character-Aware Neural Network for Distorted Scene Text Recognition[C]//AAAI. 2018. [paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/16327/16307)

**[26] \[AAAI-2018]** Liu Z, Li Y, Ren F, et al. SqueezedText: A Real-Time Scene Text Recognition by Binary Convolutional Encoder-Decoder Network[C]//AAAI. 2018. [paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/16354/16312)

**[27] \[CVPR-2018]** Bai, F, Cheng, Z, Niu, Y, Pu, S and Zhou,S. Edit probability for scene text recognition, pages 1508-1516, 2018. [paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Bai_Edit_Probability_for_CVPR_2018_paper.pdf)

**[28] \[ECCV-2018]** Liu Y, Wang Z, Jin H, et al. Synthetically Supervised Feature Learning for Scene Text Recognition[C]//Proceedings of the European Conference on Computer Vision (ECCV). 2018: 435-451. [paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Yang_Liu_Synthetically_Supervised_Feature_ECCV_2018_paper.pdf)

**[29] \[ICIP-2018]** Gao Y, Chen Y, Wang J, et al. Dense Chained Attention Network for Scene Text Recognition[C]//2018 25th IEEE International Conference on Image Processing (ICIP). IEEE, 2018: 679-683. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8451273)

**[30] \[TPAMI-2018]** Shi B, Yang M, Wang X, et al. Aster: An attentional scene text recognizer with flexible rectification[J]. IEEE transactions on pattern analysis and machine intelligence, 2018. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8395027) [code](https://github.com/bgshih/aster)

**[31] \[CVPR-2012]** A. Mishra, K. Alahari, and C. V. Jawahar. Top-down and bottom-up cues for scene text recognition. In CVPR, 2012. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6247990)

**[32] \[ICCV-2011]** K. Wang, B. Babenko, and S. Belongie. End-to-end scene text recognition. In ICCV, 2011. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6126402)

**[33] \[IJDAR-2005]** S. M. Lucas, A. Panaretos, L. Sosa, A. Tang, S. Wong, R. Young,K. Ashida, H. Nagai, M. Okamoto, H. Yamamoto, H. Miyao,J. Zhu, W. Ou, C. Wolf, J. Jolion, L. Todoran, M. Worring, and X. Lin. ICDAR 2003 robust reading competitions:entries, results,and future directions. IJDAR, 7(2-3):105–122, 2005. [paper](https://link.springer.com/content/pdf/10.1007%2Fs10032-004-0134-3.pdf)

**[34] \[ICDAR-2013]** D. Karatzas, F. Shafait, S. Uchida, M. Iwamura, L. G. i Bigorda,S. R. Mestre, J. Mas, D. F. Mota, J. Almaz ́ an, and L. de las Heras. ICDAR 2013 robust reading competition. In ICDAR, 2013. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6628859)

**[35] \[ICCV-2013]** T. Q. Phan, P. Shivakumara, S. Tian, and C. L. Tan. Recognizing text with perspective distortion in natural scenes. In ICCV, 2013. [paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Phan_Recognizing_Text_with_2013_ICCV_paper.pdf)

**[36] \[Expert Syst.Appl-2014]** A. Risnumawan, P. Shivakumara, C. S. Chan, and C. L. Tan. A robust arbitrary text detection system for natural scene images. Expert Syst. Appl., 41(18):8027–8048, 2014. [paper](https://pdf.sciencedirectassets.com/271506/1-s2.0-S0957417414X00114/1-s2.0-S0957417414004060/main.pdf?x-amz-security-token=AgoJb3JpZ2luX2VjEIn%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJGMEQCIGRhldIzSEiSi38FQg8SKy0nbkjetbYc6MOZN8lXbsg7AiB5pY6PoVDS8%2F3qS%2FPqd0zaHjqWrjqvDrAtTiZVSrpKmyrjAwiC%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAIaDDA1OTAwMzU0Njg2NSIMoRUcs%2Ft3M%2Blz7DI3KrcDKVODcJNpq1tNel77UHdAJVSUDWRkG7Fx5loyHhQsb2V3MFfHqAGKJpbdr7xHlDY7CaTl5nrTdNe91InXfpM25fFyYQlANwrhlcYGiPEsN14mSBe%2F5gy0gipiPaN835Viwb0O1Raw9MP9Clc84q%2BHvW5YyQ02NIZYE7OlHYSWN6mbI0F9r7reRa2zNLjFVcvJRkAyt4I9L1Pbehf4WwFF1Er0ResczdJ2FbwKCZNaKWznwhdjVp8hw0SFC%2F9uxnDHzu8DTPeutA3mHeUetMOEtKspkSvIj%2FWQDI1OTECcNv0N7CfmUKSh9m5tOYn%2Fb7KQx8pPA450Snd3faB7euDzPwvCmtfeUzYs0n0UxWt9JWXxKONmvrMlxf9bjZL0RBR1NNeNgwFuCCCRZDAKogbBI%2FclJmPUiNO38mHO10B1unMow9XtojodS3U6Iz2n8jeERhaR4Rt4KeWB9ojZTQhUr5d1uUX%2FVpmJmFQhgvPXmEi%2Fnlp65TXeZNdbUncQPqZ8PaKGYxJn1F%2FwnuJH1Ww6ksTur4rcggGAEHTBgXL5vmLjJG2ZhH1vxaoY8qtUO5EuXwVVfBXCtzCit9jmBTq1Abb%2BixDckXLEYAwidBhA%2B4MKpbhmH4LItnjE3tSuFgOHFbwaq9g0MZyGtL3OUxCKc3eAkkLzOrJnEag%2F2eV%2BdMcU9%2F%2BKI5h8yQsz5PEFeqkY3BID%2BY7oIU6qhqhb38PVrbt1oyF420cS%2BoSpt2Nj6E%2FuCZZTrgMakE%2B9QXvAaTIBWG%2Fc0xOv6d3rGTAnZTkkscgD7j%2FP1jqFkf388YT5jCbAWlx8OiMbj%2BVPkK8UvXhgSh1ZPMk%3D&AWSAccessKeyId=ASIAQ3PHCVTY6VYAY5FB&Expires=1557539079&Signature=HF7E%2BOACBDJPtLAerMWH6MTKDCw%3D&hash=8fe7c8a1c5599e4659a2b26919b2a59f4aff8c452e5a07793dc187e49c69dc9e&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0957417414004060&tid=spdf-7bd6a860-4c57-4e39-87ce-bd2f050badcf&sid=57f9f09d5d026341242a7bd2fb38b97c5897gxrqb&type=client)

**[37] \[ICDAR-2015]** D. Karatzas, L. Gomez-Bigorda, A. Nicolaou, S. K. Ghosh, A. D.Bagdanov, M. Iwamura, J. Matas, L. Neumann, V. R. Chandrasekhar, S. Lu, F. Shafait, S. Uchida, and E. Valveny. ICDAR 2015 competition on robust reading. In ICDAR, pages 1156–1160,2015. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7333942)

**[38] \[arXiv-2016]** Veit A, Matera T, Neumann L, et al. Coco-text: Dataset and benchmark for text detection and recognition in natural images[J]. arXiv preprint arXiv:1601.07140, 2016. [paper](https://arxiv.org/pdf/1601.07140.pdf)

**[39] \[ICDAR-2017]** Ch'ng C K, Chan C S. Total-text: A comprehensive dataset for scene text detection and recognition[C]//Document Analysis and Recognition (ICDAR), 2017 14th IAPR International Conference on. IEEE, 2017, 1: 935-942. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8270088)

**[40] \[ICDAR-2017]** Shi B, Yao C, Liao M, et al. ICDAR2017 competition on reading chinese text in the wild (RCTW-17)[C]//Document Analysis and Recognition (ICDAR), 2017 14th IAPR International Conference on. IEEE, 2017, 1: 1429-1434. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8270164)

**[41] \[ICPR-2018]** He M, Liu Y, Yang Z, et al. ICPR2018 Contest on Robust Reading for Multi-Type Web Images[C]//2018 24th International Conference on Pattern Recognition (ICPR). IEEE, 2018: 7-12. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8546143)

**[42] \[arXiv-2018]** Yuan T L, Zhu Z, Xu K, et al. Chinese Text in the Wild[J]. arXiv preprint arXiv:1803.00085, 2018. [paper](https://arxiv.org/pdf/1803.00085.pdf)

**[43] \[arXiv-2017]** Yuliang L, Lianwen J, Shuaitao Z, et al. Detecting curve text in the wild: New dataset and new solution[J]. arXiv preprint arXiv:1712.02170, 2017. [paper](https://arxiv.org/pdf/1712.02170.pdf)

**[44] \[ECCV-2018]** Yao C, Wu W. Mask TextSpotter: An End-to-End Trainable Neural Network for Spotting Text with Arbitrary Shapes.//Proceedings of the European Conference on Computer Vision (ECCV). 2018: 71-88. [paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Pengyuan_Lyu_Mask_TextSpotter_An_ECCV_2018_paper.pdf)

**[45] \[NIPS-WORKSHOP-2011]** Yuval Netzer, Tao Wang, Adam Coates, Alessandro Bissacco,Bo Wu, and Andrew YNg. Reading digits in natural images with unsupervised feature learning. In NIPS workshop on deep learning and unsupervised feature learning, volume 2011, page 5, 2011. [paper](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/37648.pdf)

**[46] \[PR-2019]**  C. Luo, L. Jin, and Z. Sun, “MORAN: A multi-object rectified attention network for scene text recognition,” Pattern Recognition, vol. 90, pp. 109–118, 2019. [paper](https://pdf.sciencedirectassets.com/272206/1-s2.0-S0031320319X00023/1-s2.0-S0031320319300263/main.pdf?x-amz-security-token=AgoJb3JpZ2luX2VjEHcaCXVzLWVhc3QtMSJIMEYCIQCceDsmz9xCoE%2FnPRGjEfK6RAdvbVW7B%2B7rvG4viZPq%2BAIhALnS8lFI9N7LE3%2BNey3EgbWZU8f%2BJIAJIxlk5ewtKNTgKtoDCG8QAhoMMDU5MDAzNTQ2ODY1IgxbFmRrlDI1X0pjiscqtwMyG%2F2gaQjY2Ol3wnc2MtQwmfUOBotnxAj7F7lPnLyeRqPWJo6swI52Tz0YWuSI%2FTXRk3wuLNZthvTkLRWlD5wejFNGIAM9VNUuaYmfhLPT%2Ft33yaDBMGBe3wP%2BdsH0OXHn7JtbzLAFK%2BFPBYXLfSMth4IbmdKzLPAR77noWqY3NvtbYRJEvpw4r9N7yvM%2Fo1lBQnoulBsX%2B7sKRKm9SxWrreldzSuX2EIbnk5FPyXAkTlzYfH%2FCjoTOGYrReZl1VeFSnml73TaF1RImYbO0t155QfM8X90oEMKxlfd1IU8PzuYy14%2Bo0TAmHB3kYh3aKN6CEZ%2FEAHhxxhGrysEhBZWLF0RMp2oZFGDPxiOJVo3QES2GR38d9uBYjXF0dzjxgFnn40SuYTRE29nIjspgjZbsqeWyP%2BbsFHJcteX3w0eN6wq%2B%2Bbd5yPuAELoAy246KPZvRwBXGYUH1%2Bgm%2BqIIKidMGUedx98L2%2FO%2FAnbQ7gPCKW9HIWRdExufStWHid2r8gPpwB3%2Fb%2FKtCbA7iqm7cedZaqgjvaBbKM0hgBlgfXMGJTniXSmGYAIhvgH0aAlUCAAGeNsovbGMMCw1OYFOrMBESogEL75zcwF5QSaTC8s2DdSVFWjhwza7lgexCXY7r6aW4Y80XYluSj6%2BPWj2x6qH23kIlPIEfmyXL%2FJbbBzxTh%2FBbA9UVu04wph8eB%2BNGtvajIx%2FZFVNJSHc3WHz2DWlSAkLnuNGtahDLdXTG3ZD9jhdbweN7QdKYXsPPLh6ysos7v0hO9f7mM2%2BWsA5yOwB8lg9d2xmYu2PU6RKCQcv8hC1ASHgZh5PiYGBUjTfdv0cfI%3D&AWSAccessKeyId=ASIAQ3PHCVTYXA3CRTFK&Expires=1557473755&Signature=eBwdaj8gPpxtBnisCTPveLqX3iw%3D&hash=6f612616f8fba56ffd779d1eee8bfb19e39b7276f2b922ed529a46e51075049d&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0031320319300263&tid=spdf-5d02711b-ea3c-46c1-bb55-4d301d13f947&sid=57f9f09d5d026341242a7bd2fb38b97c5897gxrqb&type=client) [code](https://github.com/Canjie-Luo/MORAN_v2)

**[47] \[ACM-2019]** Xie H, Fang S, Zha Z J, et al, “Convolutional Attention Networks for Scene Text Recognition,” ACM Transactions on Multimedia Computing, Communications, and Applications (TOMM), vol. 15, pp. 3 2019. [paper](https://dl.acm.org/citation.cfm?id=3231737)

**[48] \[AAAI-2019]** Liao M, Zhang J, Wan Z, et al, “Scene text recognition from two-dimensional perspective,” //AAAI. 2019. [paper](https://arxiv.org/pdf/1809.06508.pdf) 

**[49] \[AAAI-2019]** Li H, Wang P, Shen C, et al, “Show, Attend and Read: A Simple and Strong Baseline for Irregular Text Recognition,” //AAAI. 2019. [paper](https://arxiv.org/pdf/1811.00751.pdf)

**[50] \[TPAMI-2015]** Ye Q, Doermann D. Text detection and recognition in imagery: A survey[J]. IEEE transactions on pattern analysis and machine intelligence, 2015, 37(7): 1480-1500. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6945320)

**[51] \[Frontiers-Comput. Sci-2016]** Zhu Y, Yao C, Bai X. Scene text detection and recognition: Recent advances and future trends[J]. Frontiers of Computer Science, 2016, 10(1): 19-36. [paper](https://link.springer.com/article/10.1007/s11704-015-4488-0)

**[52] \[arXiv-2018]** Long S, He X, Ya C. Scene Text Detection and Recognition: The Deep Learning Era[J]. arXiv preprint arXiv:1811.04256, 2018. [paper](https://arxiv.org/pdf/1811.04256.pdf)

**[53] \[NIPS-WORKSHOP-2014]** M. Jaderberg, K. Simonyan, A. Vedaldi, A. Zisserman, Synthetic data and artificial neural networks for natural scene text recognition, in: Proceedings of Advances in Neural Information Processing Deep Learn. Workshop (NIPS-W).2014. [paper](https://arxiv.org/pdf/1406.2227.pdf)

**[54] \[CVPR-2016]** A. Gupta, A. Vedaldi, A. Zisserman, Synthetic data for text localisation in natural images, in: Proceedings of Computer Vision and Pattern Recognition (CVPR), 2016, pp. 2315–2324. [paper](http://www.robots.ox.ac.uk/~ankush/textloc.pdf)

