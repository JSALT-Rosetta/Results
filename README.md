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
| phone forced align + textUWD |   |   |   | dpseg  |
|  speechUPD + textUWD         |   |   |   | dpseg |
|  speechUWD                   |   |   |   | jensen |

* token

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  0.024 |  0.099  | 0.038  | |
|  speechUPD as W.  	         |  0.015 | 0.043   | 0.022  | |
| phone forced align + textUWD |   |   |   | dpseg |
|  speechUPD + textUWD         |   |   |   | dpseg |
|  speechUWD                   |   |   |   | jensen |

* type

| method  |  P |  R |  F | Remarks |
|---|---|---|---|---|
|  phone forced align. as W.   |  0.017 |  0.017 | 0.017  | |
|  speechUPD as W.  	         |  0.016 | 0.027  | 0.020  | |
| phone forced align + textUWD |   |   |   | dpseg |
|  speechUPD + textUWD         |   |   |   | dpseg |
|  speechUWD                   |   |   |   | jensen |

## add other results on other tasks below

new task - new dataset
