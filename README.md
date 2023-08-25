# Narrowband-channel-in-Wireless-Communication
<p align="justify"> Consider a wireless system, suppose the channel is narrowband and after sampling, the received signal at the moment 𝑚 is in the form of the following relationship: </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/a77e2304-7398-4c05-b1b2-8635e9d780f3)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/6af6b12f-7f6a-4a5b-8fe1-99d88aa97f4f)

## Part 1.
Suppose BPSK modulation is used to send data. In other words:

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/1ac71f49-d45e-4329-9022-ea623bd9a9f3)

### Part a.
Plot the graph of optimal error probability in terms of 𝑆𝑁𝑅 in the interval [−20,20]dB.

<p align="justify"> For this part, based on the given relationship and also knowing the distributions of $w[m]$ and $h[m]$, we form the final signal. The point is that to get the final signal, we have considered two real and imaginary parts and implemented it this way. The graph of the optimal error probability in this case is as follows, which, as can be seen, fluctuates around the number of 0.5 BER values. The reason for this is that in this case, the channel has fading, but the amount of fading is not known. The amount of fading can be positive or negative with equal probability, and the symbols are also sent as BPSK, so it is expected that the error values ​​are around 0.5, which was also seen in the following figure. </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/8d5242b8-25c0-4379-a9f1-f4d520e29a4e)

### Part b.
Plot the graph of the previous part in the case where the channel does not fade (in other words $h[m]=1$).

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/6eaa82af-92e8-47a3-94c7-b39a869e7d80)

### Part c.
Obtain the theoretically optimal error probability for the previous part.

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/0ec8eec7-9e5a-4e7f-b72a-07e594ca8d4c)

In $P_{e}=10^{−6}$, the SNR value in dB will be as follows:

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/b1eaede0-a3fe-458f-9a89-974bc6d479f6)

<p align="justify"> For a better comparison of the answers obtained in the previous part and this part, we have plotted together the graphs of the theoretical solution and the solution of part(b) in the figure below. </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/48bce361-437f-4c5c-bd09-bff9f6a12c43)

## Part 2.
Suppose to send bit 1 in two consecutive time intervals, symbol 0 and $\alpha$ are sent respectively.

### Part a.
<p align="justify"> Obtain the optimal decision-making method and the optimal error probability theoretically in terms of SNR and plot its graph using the relationship obtained in the interval [−20,20]dB. </p>

<p align="justify"> The difference between this question and the previous question is that we are sending two symbols for each bit. That is, the input symbols can be $x_{1}=0$  and $x_{2}=\alpha$ and vice versa. In this case, the outputs of the system will be $y_{1}$ and $y_{2}$, and the optimal decision limit in this case is $y_{1}=y_{2}$. According to these explanations, we get the probability of error as follows: </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/01a70a50-716a-4949-a4d7-8fd18bba2219)

**Note:** The difference between two Gaussian random variables with variance $N_{0}/2$ is a Gaussian random variable whose variance doubles.

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/a865c602-a9e9-40cb-b591-ffa45c1e434e)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/135014f2-85f8-4c45-a71d-4e120a6bbe76)

<p align="justify"> It should be noted that both in the relationship above and in the relationship of part(c) of the previous question, the SNR values ​​that are included in the relationship should be linear and not in decibels. </p>

Now, based on the obtained relationship, we plot the error probability diagram:

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/88b6cb13-a0d9-46d3-b8fe-b2f58cd1ca20)

### Part b.
<p align="justify"> We proceed according to the relationships we wrote in part(a) of this question and find the probability of error. In this case, to get the probability of error, the delta we form is the difference of two output signals, namely $y_{1}$ and $y_{2}$. To find the probability of error, we also check the logical vector that is created by comparing the delta with the generated bits, and based on that, we find the probability of error. </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/4f4f0534-59f0-4b52-a57c-a9b864d1e162)

The previous plots are somhow similar and if we plot them together we can see their resemblance.

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/56f7ff25-eafb-4383-b5dc-f5363264438d)

### Part c.
Now we want to calculate the value of SNR in which the probability error is $10^{-6}$.

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/de5fd1ff-dd46-4dc4-8ac4-31201ca420d9)

<p align="justify"> The calculated values ​​in this question and the previous question differ by almost 3dB. The result is that in an equal probability of error for the system of questions 1 and 2, the amount of SNR required in the second system should be higher, and this means that the power sent in the second system is higher. </p>

## Part 3.
















