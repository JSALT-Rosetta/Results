# Update on JSALT Results

## un-supervised word discovery on mboshi dataset 

speechUWD: Jensen’s segmental DTW word discovery (Baseline)

speechUPD: Un-supervised Phone discovery (Markus or Lucas)

textUWD: Un-supervised word discovery from text (Pierre)

phone forced align : Forced-alignment between speech and mboshi transcripts - 27 phone units (Topline)

markus : boundary detection + articulatory features (AF) clustering

lucas : bayesian phone loop


* NED/Cov

| method  |  NED |  COV |  Remarks |
|---|---|---|---|
|  phone forced align. as W.   |  0 |  100  | |
|  speechUPD as W.  	       |  xx.x |  xx.x  | markus (22 units) |
|  speechUPD as W.  	       |  92.7 |  97.8  | lucas MFCC (max 100 units) |
| phone forced align + textUWD |  0 |  100  | dpseg topline |
| phone forced align + textUWD |  0 |  99.5  | attention (fr-mb)  |
| phone forced align + textUWD |  0 |  99.2  | attention (mb-fr)  |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (5 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (10 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (15 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (20 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (22 units) + dpseg* |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (30 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (40 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (50 units) + dpseg |
|  speechUPD + textUWD         |  xx.x |  xx.x  | markus (60 units) + dpseg |
|  speechUPD + textUWD         |  93.4 | 97.8      | lucas (max 100 units) + dpseg |
|  speechUPD + textUWD         |  92.5 | 96.1      | lucas (max 100 units) + attention (fr-mb) |
|  speechUPD + textUWD         |  91.2 | 97.3      | lucas (max 100 units) + attention (mb-fr) |
|  speechUWD                   |  27.6 | 28.6   | jansen |


* boundary

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  30.4 |  100 | 46.6  | |
|  speechUPD as W.  	       |  20.9 | 52.5  | 29.9  | markus (22 units) |
|  speechUPD as W.  	       |  23.9 | 81.0  | 36.9  | lucas HMM MFCC (max 100 units) |
|  speechUPD as W.  	       |  25.2 | 80.2  | 38.4  | lucas HMM MBN (max 100 units) |
|  speechUPD as W.  	       |  26.0 | 68.2  | 37.6  | lucas HMM MBN (max 48 units) TIMIT pretrain (no adaptation) |
|  speechUPD as W.  	       |  28.0 | 72.3  | 40.4  | lucas HMM MBN (max 48 units) TIMIT pretrain |
|  speechUPD as W.  	       |  28.2 | 72.5  | 40.6  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain |
|  speechUPD as W.  	       |  28.7 | 74.2  | 41.4  | lucas SVAE2 HMM MBN (max 48 units) TIMIT pretrain |
| phone forced align + textUWD |  68.2 |  82.6 | 74.7  | dpseg topline |
| phone forced align + textUWD |  51.7 |  67.9 | 58.7  | attention (fr-mb) |
| phone forced align + textUWD |  41.1 |  52.1 | 45.9  | attention (mb-fr) |
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
|  speechUPD + textUWD         | 29.3  | 66.4  | 40.7  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + dpseg |
|  speechUPD + LatticeUWD      | 30.9  | 61.4  | 41.1  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + latticeUWD |
|  speechUPD + textUWD         | 36.6  |  43.2 | 39.6  | lucas (max 100 units) + attention (fr-mb) |
|  speechUPD + textUWD         | 34.7  |  43.6 | 38.6  | lucas (max 100 units) + attention (mb-fr) |
|  speechUPD + textUWD         | 44.0  | 38.5  | 41.1  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + attention (fr-mb) 
|  speechUPD + textUWD         | 40.4  | 41.6  | 41.0  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + attention (mb-fr) 
|  speechUWD                   |  27.3 | 12.0  | 16.6  | jensen |

* token

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  2.4 |  9.9  | 3.8  | |
|  speechUPD as W.  	       |  1.5 | 4.3   | 2.2  | markus |
|  speechUPD as W.  	       |  1.4 | 7.0   | 2.4  | lucas HMM MFCC (max 100 units) |
|  speechUPD as W.  	       |  1.5 | 6.7   | 2.5  | lucas HMM MBN (max 100 units)  |
|  speechUPD as W.  	       |  2.3 | 7.5   | 3.5  | lucas HMM MBN (max 48 units) TIMIT pretrain (no adaptation) |
|  speechUPD as W.  	       |  2.1 | 7.0   | 3.2  | lucas HMM MBN (max 48 units) TIMIT pretrain |
|  speechUPD as W.  	       |  2.1 | 7.2   | 3.3  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain |
|  speechUPD as W.  	       |  2.2 | 7.4   | 3.4  | lucas SVAE2 HMM MBN (max 48 units) TIMIT pretrain |
| phone forced align + textUWD | 34.3 | 41.3  | 37.5  | dpseg topline |
| phone forced align + textUWD |  15.9 |  22.2 | 18.5  | attention (fr-mb) |
| phone forced align + textUWD |  5.2 |  7.0 | 6.0  | attention (mb-fr) |
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
|  speechUPD + textUWD         | 2.3  | 6.7  | 3.5  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + dpseg |
|  speechUPD + latticeUWD      | 2.4 | 6.0   | 3.4  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + latticeUWD |
|  speechUPD + textUWD         | 3.1  |  4.0 |  3.5 | lucas (max 100 units) + attention (fr-mb) |
|  speechUPD + textUWD         | 2.7  |  3.8 |  3.1 | lucas (max 100 units) + attention (mb-fr) |
|  speechUPD + textUWD         | 2.7  | 2.4  | 2.6  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + attention (fr-mb) 
|  speechUPD + textUWD         | 3.2  | 3.7  | 3.5  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + attention (mb-fr) 
|  speechUWD                   | 2.3  | 0.9  | 1.3  | jensen |

* type

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  1.7 |  1.7 | 1.7  | |
|  speechUPD as W.  	         |  1.6 | 2.7  | 2.0  |markus |
|  speechUPD as W.  	         |  1.8 | 2.7  | 2.2  | lucas HMM MFCC (max 100 units) |
|  speechUPD as W.  	         |  1.6 | 2.5  | 1.9  | lucas HMM MBN (max 100 units)  |
|  speechUPD as W.  	         |  2.0 | 3.4  | 2.5  | lucas HMM MBN (max 48 units) TIMIT pretrain (no adaptation) |
|  speechUPD as W.  	         |  2.0 | 3.5  | 2.6  | lucas HMM MBN (max 48 units) TIMIT pretrain |
|  speechUPD as W.  	         |  2.1 | 3.7  | 2.7  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain |
|  speechUPD as W.  	         |  2.1 | 3.6  | 2.6  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain |
| phone forced align + textUWD | 21.4  | 28.2  | 24.3  | dpseg |
| phone forced align + textUWD |  13.1 |  22.9 | 16.7  | attention (fr-mb) |
| phone forced align + textUWD |  4.9 |  9.9 | 6.6  | attention (mb-fr) |
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
|  speechUPD + textUWD         | 2.3  | 4.4  | 3.1  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + dpseg |
|  speechUPD + LatticeUWD      |  2.8 | 5.3  | 3.6  |lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + latticeUWD |
|  speechUPD + textUWD         | 3.5  | 6.4  |  4.5 | lucas + attention (fr-mb) |
|  speechUPD + textUWD         | 3.1  | 6.3  |  4.2 | lucas + attention (mb-fr) |
|  speechUPD + textUWD         | 2.9  | 4.1  | 3.4  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + attention (fr-mb) 
|  speechUPD + textUWD         | 3.5  | 6.5  | 4.6  | lucas SVAE HMM MBN (max 48 units) TIMIT pretrain + attention (fr-mb) 
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


## French-to-Mboshi Translation 

sys1:  generate real mboshi symbols (grapheme units similar to Markus’ forced-alignments units)

sys2:  generate lucas’ mboshi pseudo symbols (so this system only uses french_txt + mboshi_speech as parallel data !!)

same train/dev protocol for both systems (4643utt/514utt) - BLEU4 eval (on phones or pseudo phones)

| dataset | sys1 (BLEU4) | sys2 (BLEU4) |
|---------|--------|-----|
| train | 48.80 |  19.12 |
| dev | 31.95 |  8.32 |



## Mboshi Speech Transcription / Translation 

same train/dev/tst protocol for all systems (4643utt/257utt/257utt) - config (b) by Pierre

see /pylon5/ci560op/godard/xnmt/output/mboshi-xp1

|   | BLEU4/BLEU1  | BLEU4/BLEU1 | Char ER  | Char ER | Word ER  | Word ER |
|---------|--------|--------|--------|--------|--------|--------|
|   | dev  | tst | dev  | tst | dev  | tst |
| Transcript. (Mb car)  | 45.58/-  | 13.84/- | 51.05  | 81.15 | -  | - |
| Translate (Fr car)  | 20.99/-  | 12.26/- | 80.65  | 85.42 |  -  | - |
| Translate (Fr words) | 7.51/18.37  | 0.0/11.88 | 79.61  | 84.53 | 96.98  | 110.28 |









## add other results on other tasks below

new task - new dataset
