

### AlexNet: Feature Map Size Calculation

How the input image of size $224 \times 224$ changes across layers.

The formula used for convolution and pooling layers:

$H_{out} = \left\lfloor \frac{H + 2P - K}{S} \right\rfloor + 1$

where:
- $H$ = input height/width  
- $K$ = kernel size  
- $S$ = stride  
- $P$ = padding  

---

#### Input
 
$3 \times 224 \times 224$ [channel, width, height]

---

#### Conv1: in_channels=$3 \rightarrow$ out_channel=$64$, $K=11$, $S=4$, $P=2$

$H_{out} = \left\lfloor \frac{224 + 2 \cdot 2 - 11}{4} \right\rfloor + 1 = 55$

Output: $64 \times 55 \times 55$

---

#### MaxPool1: $K=3$, $S=2$

$H_{out} = \left\lfloor \frac{55 - 3}{2} \right\rfloor + 1 = 27$

Output: $64 \times 27 \times 27$

---

#### Conv2: $64 \rightarrow 192$, $K=5$, $S=1$, $P=2$

$H_{out} = \left\lfloor \frac{27 + 2 \cdot 2 - 5}{1} \right\rfloor + 1 = 27$

Output: $192 \times 27 \times 27$

---

#### MaxPool2: $K=3$, $S=2$

$H_{out} = \left\lfloor \frac{27 - 3}{2} \right\rfloor + 1 = 13$

Output: $192 \times 13 \times 13$

---

#### Conv3: $192 \rightarrow 384$, $K=3$, $S=1$, $P=1$

$H_{out} = \left\lfloor \frac{13 + 2 \cdot 1 - 3}{1} \right\rfloor + 1 = 13$

Output: $384 \times 13 \times 13$

---

#### Conv4: $384 \rightarrow 256$, $K=3$, $S=1$, $P=1$

Output: $256 \times 13 \times 13$

---

#### Conv5: $256 \rightarrow 256$, $K=3$, $S=1$, $P=1$

Output: $256 \times 13 \times 13$

---

#### MaxPool3: $K=3$, $S=2$

$H_{out} = \left\lfloor \frac{13 - 3}{2} \right\rfloor + 1 = 6$

Output: $256 \times 6 \times 6$

---

#### Flatten

$256 \times 6 \times 6 = 9216$

---

#### Fully Connected Layer

Input to first linear layer: $9216$
