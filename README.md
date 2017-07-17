# Update on JSALT Results

## un-supervised word discovery on mboshi dataset 

speechUWD: Jensen’s segmental DTW word discovery (Baseline)

speechUPD: Un-supervised Phone discovery (Markus or Lucas or ??)

textUWD: Un-supervised word discovery from text (Pierre)

phone forced align : Forced-alignment between speech and mboshi transcripts (Topline)


* boundary

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  0.304 |  1.000 | 0.466  | |
|  speechUPD as W.  	         |  0.209 | 0.525  | 0.299  | markus |
| phone forced align + textUWD |  0.682 |  0.826 | 0.747  | dpseg  |
|  speechUPD + textUWD         |  0.214 | 0.493  | 0.298  | markus + dpseg |
|  speechUPD + textUWD         |   |   |   | lucas + dpseg |
|  speechUWD                   |   |   |   | jensen |

* token

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  0.024 |  0.099  | 0.038  | |
|  speechUPD as W.  	         |  0.015 | 0.043   | 0.022  | |
| phone forced align + textUWD |  0.343 | 0.413  | 0.375  | dpseg |
|  speechUPD + textUWD         | 0.013  | 0.041  | 0.020  | markus + dpseg |
|  speechUPD + textUWD         |   |   |   | lucas + dpseg |
|  speechUWD                   |   |   |   | jensen |

* type

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  0.017 |  0.017 | 0.017  | |
|  speechUPD as W.  	         |  0.016 | 0.027  | 0.020  | |
| phone forced align + textUWD | 0.214  | 0.282  | 0.243  | dpseg |
|  speechUPD + textUWD         | 0.017  | 0.033  | 0.023  | markus + dpseg |
|  speechUPD + textUWD         |   |   |   | lucas + dpseg |
|  speechUWD                   |   |   |   | jensen |

## add other results on other tasks below

new task - new dataset
