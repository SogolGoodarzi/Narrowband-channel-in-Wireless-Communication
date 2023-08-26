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
Now suppose that the channel information (values ​​of $h[m]$) is fully known. Suppose BPSK modulation is used to send data. In other words:

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/4bc28da7-2804-44e5-b3eb-aefebb072518)

### Part a.
<p align="justify"> Obtain the optimal decision making method in the receiver as well as the optimal error probability of detecting the $x[m]$ symbol in the receiver theoretically in terms of $h[m]$ and the amount of SNR, and then obtain the average value of the error probability in terms of SNR and plot it in the interval [−20,20]dB. We can eliminate the effect of the channel by multiplying a factor or coefficient in the equation of the system. This work is similar to water filling or equalization. So we will have: </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/026f851b-2ea8-4131-950b-5ebbadb9cec9)

Now we need to get the new noise variance. In this case, we will have according to the relation above:

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/4f3d7e27-a941-410c-a74b-e0cfdd7c3a25)

If the gain of the channel (h) has Rayleigh distribution, then we have a probability of error to calculate the average:

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/d6e9c72d-a68d-476a-8470-6eddf1ccc304)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/4952cd6b-290c-4c30-af74-c2ca90813634)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/7be848b5-6c35-4916-8ec3-d098d91adee3)

Now, based on the relationship obtained above, we plot the average error probability diagram as follows:

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/e8e0f6d3-44bb-4cd8-bd85-c20a96867525)

Based on manual calculations in $P_{e}=10^{−6}$, the SNR value in dB will be as follows:

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/edb6c882-d86c-472b-b0fb-3672a1294ded)

### Part b.
<p align="justify"> Therefore, in part(a) we eliminated the effect of the channel by multiplying the appropriate coefficient, we follow the same process for simulation and find the probability of error. (Relationships required for better understanding are placed in the simulation file.) So we will have the obtained error probability diagram as follows. </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/80a40ce2-0585-4f26-9741-2936f29e824d)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/d5bda355-b2df-4efb-a910-fd6a6a3dc059)

<p align="justify"> Since the range of SNR for plotting graphs is from -20dB to 20dB, as a result, the SNR is sufficiently large, meaning SNR = 20dB. In this SNR, we should compare the error probability values ​​of two graphs. In the figure below, the error probability values ​​at this point are specified for two graphs. </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/4f26b3cb-94a3-47e6-ab25-6cfc9efb7668)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/04280cbe-4b96-477c-b285-cd2b72f8f7e0)

We can see that the difference between the graphs at high SNR is almost 24 dB.

### Part c.
<p align="justify"> As it is clear from figures, knowing the channel information reduces the possibility of error. This means that at higher SNRs, as can be seen in the figure, the error probability when the channel information is known is lower than when the channel is not available. </p>

<p align="justify"> In part A of the first question, we saw that if the channel had fading but its information was not available, the probability of error was around 0.5, but in the case that the channel has fading and its information is known, the probability of error even reaches less than 0.5 and this means that having channel information improves the possibility of system error. The point is that when we have fading in the channel and we can estimate this fading, we have a poorer performance than when we don't have fading. The reason for this is that the coefficient that we multiply to eliminate fading (similar to what we did in part A of this question) increases the variance and power of the noise. </p>

## Part 4.
As in part 3, suppose the information of the involved channel is known. Suppose QPSK modulation is used to send data. 

### Part a.
Plot the graph of the error probability in terms of SNR both theoretically and by simulation and plot them in the interval [−20,20]dB.

<p align="justify"> To simulate QPSK modulation, we use the equivalence of this modulation with two BPSK modulations. In this case, symbols $s_1$ and $s_2$ are symbols of BPSK modulation. The point that should be taken into account and observed in the simulations is that $N_0$ here is the variance corresponding to the noise that is related to the QPSK modulation, as a result, to form the noise matrices (which have two real and imaginary parts), the noise variance which should be considered is $N_0/4$. (Actually, for each of the BPSK modulations, the noise variance is $N_0/2$. On the other hand, we have two real and imaginary parts for noise, as a result, the variance of each part will be half of this value). Now, based on the above explanation, we will calculate the probability of error in the same way as part(a) of the previous question, with the difference that here we have QPSK modulation. </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/4dc88bca-84db-4770-9d68-fb17e01deda1)

<p align="justify"> In the general relationship above, 𝑃𝑐(𝑠1 & 𝑠2) is the probability of correctly recognizing the output symbols. In this case, considering the independence of the transmitted symbols, we have: </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/29137517-25b1-4ce8-8599-163639ffcfaf)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/bc69cebe-ca9b-4ee1-852e-4cff2785c366)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/673ccc56-0e1e-4add-8110-a14af64b62be)

<p align="justify"> So, to plot the error probability diagram according to the theoretical solution, the above relationship should be used. To calculate the probability of error based on simulating the general process, we have the third question, with the difference that because here we actually send 4 symbols, as a result, the variance of the noise vectors we form will be $N_0/4$. (The noise vectors formed in the code of this section are three-dimensional vectors whose third dimension corresponds to the two symbols $s_1$ and $s_2$ that we have formed. By forming the output vectors $y_1$ and $y_2$, we form the variable $P-c$ which is the probability of correctly recognizing the symbols (according to the process we had in solving the theory) and we find the error probability based on it. The error probability diagrams of these two methods are shown in the figure below. As it is known, there is only a slight difference between these two graphs, and it can be concluded that the theoretical solution and the simulation almost end up with the same result. </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/7cf81e39-ffc9-44ce-ae7a-fd80f500fc3a)

### Part b.
<p align="justify"> Now we plot the graphs obtained in this question and the fourth question together and get the error probabilities at high SNR values ​​and calculate their difference. </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/8c9d975b-1673-4b26-81f2-00f0132f0a92)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/947c3492-678c-4b09-a938-a0cf3c65d97b)

We can see that the difference between the graphs at high SNR is almost 28 dB.

The general result is that the error probability values ​​for QPSK modulation are higher than those for BPSk modulation.

## Part 5.
<p align="justify"> In this question, we want to use the time diversity method. Suppose to send the symbol $x$ for $L$ times, we send this symbol and then reveal this symbol at the receiver. In other words, the received signal in the 𝑖-th transmission is as follows: </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/a915dd28-01c6-4d93-bdd7-12ad91e740d4)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/168c203a-acd0-479f-af3c-aafa4154af84)

### Part a.
<p align="justify"> Since the purpose of this question is to have diversity in the time domain, as a result, the information of two consecutive time slots should be independent of each other. In this case, according to the course material, it is necessary that the time between two sending symbols is $T_c$. That is, to send data in this channel, we must consider the minimum correlation time interval. </p>

### Part b.
Suppose we have used BPSK modulation in the transmitter. In other words:

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/f303f26c-390c-4be0-b681-4fa0e388bd34)

<p align="justify"> Obtain the optimal decision-making method and also the optimal error probability in terms of SNR, and then using the obtained relationship and by simulating the error probability for each 𝐿 ∈ {1,2,3,4,5} according to SNR in the range [-10,10]dB plot the corresponding graphs. </p>

<p align="justify"> Since we send the signal L times, we use the MRC method in the receiver. For this purpose, we must first cophase the received signals and in order to eliminate the channel effect, the coefficients used in this section must be $h^{*}$. In this case we will have: </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/a3d68de1-e352-40ce-b725-8c99872a638b)

<p align="justify"> By multiplying the said coefficient for cophasing, it is natural that the mean and variance of the output signal will change. According to the above relationship, we will have the distribution of ̅𝑦 as follows: </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/df0c6dfc-2b4b-46e1-af9d-4d599915fd53)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/d924e4a2-01d9-4138-8af6-cd2e419f21ef)

<p align="justify"> Now, for averaging, we must do the same as the third and fourth questions. For this purpose, we must first obtain the distribution of the random variable $|h_{i}|^{2}$. Since the distribution of $h_{i}$ s is of the Rayleigh distribution type. According to the course materials $|h_{i}|^{2}$ has an exponential distribution. Radical of this random variable is Nakagami distribution. If we take the same process of solving the third question, then we have: </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/ded68672-9c4d-4be9-a54e-e84bbe1abc85)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/8068a65b-d0e8-49cf-9ee8-2a43f68f266b)

<p align="justify"> For the simulation part, using a diversity loop, we consider the signals sent by the transmitter and plot the error probability diagram. The function written in this section works in such a way that it finds the probability of error for each L. Here too, the noise and channel matrices are three-dimensional, the third dimension of which is considered for the implementation of Tx diversity. According to the relationships written in the code file, in order to create cophasing, the input signal must be multiplied by the second power of the channel matrix size, and the noise must be multiplied by the conjugate of the channel matrix. Finally, similar to before, we form the output signal by comparing it with the input signal, we find the probability of error. The diagram plotted from the simulation is as follows. </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/37857b00-cb59-4d80-9f5d-12ed5c5cb1b4)

<p align="justify"> The general conclusion that can be drawn from the graph above is that the higher L is, the less likely the error is, and we can see that the graphs are more descending (for L=5, the graph is descending with a larger slope, but for L=1, the graph is descending with a gentler slope). </p>

## Part 6.
<p align="justify"> In this question, we want to use diversity in place. Suppose we have 𝑀 antennas in the receiver and one antenna in the transmitter. Assume that the receiving antennas are far enough apart so that the channel gains are independent of each other. For example, if 𝑀 = 2, then the received signal in the 𝑚 time interval is as follows: </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/75889532-2881-4db1-9b6d-57fe36c4da84)

### Part a.
<p align="justify"> In order to implement the system of the fifth question in this section, that is, to include time diversity, you can use Alamuti code. That is, to send consecutive symbols in a combined form in two consecutive time intervals in such a way that the effect of the channel in the output is lost and the goal of spatial diversity (in terms of the presence of multiple transmitter antennas) is achieved. Now, in order to be able to simulate the system of question five based on this method, we must give the same symbols to both transmitter antennas in order to have a linear combination of one input at the output and to be able to check the combination methods. </p>

### Part b.
<p align="justify"> Assume 𝑀 = 2 and assume the modulation at the transmitter is BPSK. To send the symbol $x_1$ and $x_2$, use Alamouti code and plot the probability of error in the receiver in the interval [-20,20]dB using optimal decision making. </p>

<p align="justify"> Tips: During the lesson, we saw that in the Alamouti method, two consecutive time intervals are used to send two symbols $u_1$ and $u_2$. More precisely, in the mth time interval $x_{1}[m]=u_1$ and $x_{2}[m]=u_2$ and in the next time interval $x_{1}[m+1]=-u_{2}^{*}$ and $x_{2}[m+1]=u_{1}^{*}$ is selected. It is also assumed that the gain of the channel is constant in these two consecutive time periods, i.e. $h_{1}[m]=h_{1}[m+1]=h_{1}$ and also $h_{2}[m]=h_{2}[m+1]=h_{2}$, in this case the received signal in these two time periods is as follows. </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/931f79ef-9b49-4ff8-9cb4-6e100c59f838)

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/e6935489-e8b3-4510-a9ff-4e9cda97cbf0)

<p align="justify"> Based on the given guidance, we proceed with the simulation. First, according to the implementation of the previous sections, we form the noise vector and the vector of $N_0$ values, then we form the noise and channel matrices for both time slots that correspond to sending two symbols $u_1$ and $u_2$. Since it has been said that the modulation is BPSK in the transmitter, as a result, to form the symbols $u_1$ and $u_2$ we act similar to the previous sections. In the next step, by forming the output signals based on the relationship given in the case of the problem, we form the estimated output symbols $s_1$ and $s_2$ with the linear combinations that were mentioned in the lesson and compare them with the original input symbols and we calculate and plot the probability of error as below. </p>

![image](https://github.com/SogolGoodarzi/Narrowband-channel-in-Wireless-Communication/assets/125180530/2ff6a732-44ed-49a2-8064-b513a0ae452a)

It can be seen that the probability of error has increased and the reason can be the increase of noise power.

### Part c.
Explain what advantage(s) the method of part(b) has over question(5) for 𝐿 = 2 in terms of error probability and sending rate.

<p align="justify"> By comparing the error probability graphs plotted in this section and section(b) of the previous question, we see that in this case, the error has taken larger values ​​than the previous case. In this case, if we want to have the same probability of error in two modes (temporal and spatial diversity), it is necessary that the SNR is higher in the spatial diversity mode. In other words, we should increase the input power compared to the noise power so that in the spatial diversity mode, the probability of error is equal to that of the temporal diversity mode. To compare the two modes in terms of data transmission rate, it can also be said that since Almouti code method is an optimal method, it sends data at a higher speed, so in this case, the speed of data transmission is higher and it is better than the fifth question. </p>
