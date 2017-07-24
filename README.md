# Update on JSALT Results

## un-supervised word discovery on mboshi dataset 

speechUWD: Jensen’s segmental DTW word discovery (Baseline)

speechUPD: Un-supervised Phone discovery (Markus or Lucas)

textUWD: Un-supervised word discovery from text (Pierre)

phone forced align : Forced-alignment between speech and mboshi transcripts - 27 phone units (Topline)


* boundary

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  30.4 |  100 | 46.6  | |
|  speechUPD as W.  	         |  20.9 | 52.5  | 29.9  | markus |
| phone forced align + textUWD |  68.2 |  82.6 | 74.7  | dpseg  |
|  speechUPD + textUWD         |  21.4 | 49.3  | 29.8  | markus (22 units) + dpseg |
|  speechUPD + textUWD         |   |   |   | lucas + dpseg |
|  speechUWD                   |  27.3 | 12.0  | 16.6  | jensen |

* token

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  0.024 |  0.099  | 0.038  | |
|  speechUPD as W.  	         |  0.015 | 0.043   | 0.022  | |
| phone forced align + textUWD |  0.343 | 0.413  | 0.375  | dpseg |
|  speechUPD + textUWD         | 0.013  | 0.041  | 0.020  | markus (22 units) + dpseg |
|  speechUPD + textUWD         |   |   |   | lucas + dpseg |
|  speechUWD                   |   |   |   | jensen |

* type

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  0.017 |  0.017 | 0.017  | |
|  speechUPD as W.  	         |  0.016 | 0.027  | 0.020  | |
| phone forced align + textUWD | 0.214  | 0.282  | 0.243  | dpseg |
|  speechUPD + textUWD         | 0.017  | 0.033  | 0.023  | markus (22 units) + dpseg |
|  speechUPD + textUWD         |   |   |   | lucas + dpseg |
|  speechUWD                   |   |   |   | jensen |

* Alan's TTS (Mean Cepstral Distorsion - MCD score) - on 1234 utt. of a single speaker (kouarata)

| method  |  MCD | Remarks |
|---|---|---|
|  phone forced align.    |  5.25  | |
|  speechUPD 	         |  5.78  | markus (22 units) |
|  speechUPD + textUWD         |  5.72 | markus (22 units) + dpseg |



## add other results on other tasks below

new task - new dataset
