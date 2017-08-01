# Update on JSALT Results

## un-supervised word discovery on mboshi dataset 

speechUWD: Jensen’s segmental DTW word discovery (Baseline)

speechUPD: Un-supervised Phone discovery (Markus or Lucas)

textUWD: Un-supervised word discovery from text (Pierre)

phone forced align : Forced-alignment between speech and mboshi transcripts - 27 phone units (Topline)

markus 22 units : ???


* NED/Cov

| method  |  NED |  COV |  Remarks |
|---|---|---|---|
|  phone forced align. as W.   |  xx.x |  xx.x  | |
|  speechUPD as W.  	         |  xx.x |  xx.x  | markus (22 units) |
|  speechUPD as W.  	         |  xx.x |  xx.x  | lucas (max 100 units) |
| phone forced align + textUWD |  xx.x |  xx.x  | dpseg topline |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (5 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (10 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (15 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (20 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (22 units) + dpseg* |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (30 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (40 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (50 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (60 units) + dpseg |
|  speechUPD + textUWD         |       |        | lucas (max 100 units) + dpseg |
|  speechUWD                   |  27.6 | 28.6   | jansen |


* boundary

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  30.4 |  100 | 46.6  | |
|  speechUPD as W.  	         |  20.9 | 52.5  | 29.9  | markus (22 units) |
|  speechUPD as W.  	         |  23.9 | 81.0  | 36.9  | lucas (max 100 units) |
| phone forced align + textUWD |  68.2 |  82.6 | 74.7  | dpseg topline |
|  speechUPD + textUWD         |  22.5 | 39.0  | 28.5  | markus (5 units) + dpseg |
|  speechUPD + textUWD         |  21.9 | 43.8  | 29.2  | markus (10 units) + dpseg |
|  speechUPD + textUWD         |  21.5 | 46.2  | 29.4  | markus (15 units) + dpseg |
|  speechUPD + textUWD         |  21.2 | 48.1  | 29.4  | markus (20 units) + dpseg |
|  speechUPD + textUWD         |  21.4 | 49.3  | 29.8  | markus (22 units) + dpseg* |
|  speechUPD + textUWD         |  21.1 | 51.1  | 29.9  | markus (30 units) + dpseg |
|  speechUPD + textUWD         |  21.1 | 51.5  | 29.9  | markus (40 units) + dpseg |
|  speechUPD + textUWD         |  21.1 | 52.1  | 30.0  | markus (50 units) + dpseg |
|  speechUPD + textUWD         |  21.0 | 52.4  | 30.0  | markus (60 units) + dpseg |
|  speechUPD + textUWD         | 25.3  |  77.5 | 38.1  | lucas (max 100 units) + dpseg |
|  speechUWD                   |  27.3 | 12.0  | 16.6  | jensen |

* token

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  2.4 |  9.9  | 3.8  | |
|  speechUPD as W.  	         |  1.5 | 4.3   | 2.2  | markus |
|  speechUPD as W.  	         |  1.4 | 7.0   | 2.4  | lucas |
| phone forced align + textUWD | 34.3 | 41.3  | 37.5  | dpseg |
|  speechUPD + textUWD         | 1.7  | 3.3  | 2.2  | markus (5 units) + dpseg |
|  speechUPD + textUWD         | 1.6  | 3.9  | 2.3  | markus (10 units) + dpseg |
|  speechUPD + textUWD         | 1.6  | 4.2  | 2.3  | markus (15 units) + dpseg |
|  speechUPD + textUWD         | 1.6  | 4.5  | 2.4  | markus (20 units) + dpseg |
|  speechUPD + textUWD         | 1.3  | 4.1  | 2.0  | markus (22 units) + dpseg* |
|  speechUPD + textUWD         | 1.6  | 4.7  | 2.4  | markus (30 units) + dpseg |
|  speechUPD + textUWD         | 1.6  | 4.8  | 2.4  | markus (40 units) + dpseg |
|  speechUPD + textUWD         | 1.5  | 4.8  | 2.4  | markus (50 units) + dpseg |
|  speechUPD + textUWD         | 1.5  | 4.8  | 2.4  | markus (60 units) + dpseg |
|  speechUPD + textUWD         | 1.6  |  6.8 |  2.6 | lucas (max 100 units) + dpseg |
|  speechUWD                   | 2.3  | 0.9  | 1.3  | jensen |

* type

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  1.7 |  1.7 | 1.7  | |
|  speechUPD as W.  	         |  1.6 | 2.7  | 2.0  |markus |
|  speechUPD as W.  	         |  1.8 | 2.7  | 2.2  |lucas |
| phone forced align + textUWD | 21.4  | 28.2  | 24.3  | dpseg |
|  speechUPD + textUWD         | 1.9  | 3.7  | 2.5  | markus (5 units) + dpseg |
|  speechUPD + textUWD         | 1.8  | 3.4  | 2.3  | markus (10 units) + dpseg |
|  speechUPD + textUWD         | 1.6  | 3.1  | 2.1  | markus (15 units) + dpseg |
|  speechUPD + textUWD         | 1.7  | 3.2  | 2.2  | markus (20 units) + dpseg |
|  speechUPD + textUWD         | 1.7  | 3.3  | 2.3  | markus (22 units) + dpseg* |
|  speechUPD + textUWD         | 1.6  | 2.9  | 2.1  | markus (30 units) + dpseg |
|  speechUPD + textUWD         | 1.6  | 3.0  | 2.1  | markus (40 units) + dpseg |
|  speechUPD + textUWD         | 1.6  | 2.9  | 2.0  | markus (50 units) + dpseg |
|  speechUPD + textUWD         | 1.6  | 2.8  | 2.0  | markus (60 units) + dpseg |
|  speechUPD + textUWD         | 1.9  | 3.0  |  2.3 | lucas + dpseg |
|  speechUWD                   |  3.1 | 1.7  |  2.2 | jensen |

* Alan's TTS (Mean Cepstral Distorsion - MCD score) - on 1234 utt. of a single speaker (kouarata)

| method  |  MCD | Remarks |
|---|---|---|
|  phone forced align.    |  5.25  | |
|  phone forced align. + text UWD   |  5.26  | word info does not help here|
|  speechUPD 	         |  5.78  | markus (22 units) |
|  speechUPD + textUWD         |  5.72 | markus (22 units) + dpseg |
|  speechUPD 	         |  5.76  | markus (5 units) |
|  speechUPD + textUWD         |  5.85 | markus (5 units) + dpseg |
|  speechUPD 	         |  5.57  | markus (10 units) |
|  speechUPD + textUWD         |  5.61 | markus (10 units) + dpseg |
|  speechUPD 	         |  5.72  | markus (20 units) |
|  speechUPD + textUWD         |  5.79 | markus (20 units) + dpseg |
|  speechUPD 	         |  5.64  | markus (30 units) |
|  speechUPD + textUWD         |  5.69 | markus (30 units) + dpseg |
|  speechUPD 	         |  5.71  | markus (40 units) |
|  speechUPD + textUWD         |  5.75 | markus (40 units) + dpseg |
|  speechUPD 	         |  5.90  | markus (50 units) |
|  speechUPD + textUWD         |  5.89 | markus (50 units) + dpseg |
|  speechUPD 	         |  5.76  | markus (60 units) |
|  speechUPD + textUWD         |  5.78 | markus (60 units) + dpseg |
|  speechUPD 	         |  5.15  | lucas (max 100 units) |
|  speechUPD + textUWD         |  5.19 | lucas (max 100 units) + dpseg |


## speech2img retrieval
| dataset | method (software) | settings | R@5 | R@10 |
|---------|--------|------|-----|-----|
| 200 examples from flickr8k test | <a href="https://github.com/neulab/jsalt-rosetta/tree/master/speech2image">tensorflow HG16</a> | default | NA | 10% |
| flickr8k test | <a href="https://github.com/neulab/xnmt/tree/hidden_states_mingxing/xnmt">xnmt HG16</a> | default | 5% | NA |
| flickr8k test | <a href="https://github.com/neulab/jsalt-rosetta/blob/master/xnmt-config/flickr40k_retrieval_longerbidir.yaml">xnmt HG16 bidirectional loss</a> |  | NA | 10% |
|---------|--------|------|-----|------|

## img2phn phone sequence generation
| dataset | method (software) | settings | BLEU4 (1/2/3/4) |
|---------|--------|------|-----|
| flickr8k dev | <a href="https://github.com/neulab/jsalt-rosetta/blob/master/xnmt-config/flickr40k_im2ph.yaml">im2ph</a> | default, epoch 27 | 0.157 (0.540/0.221/0.118/0.062) |
| flickr8k dev | <a href="https://github.com/neulab/jsalt-rosetta/blob/master/xnmt-config/flickr40k_im2ph.yaml">im2ph</a> | 64d attender, epoch 25 | 0.157 (0.544/0.225/0.122/0.064) |
|---------|--------|------|-----|





## add other results on other tasks below

new task - new dataset
