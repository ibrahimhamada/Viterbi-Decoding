# Implementation-of-Viterbi-Decoding

# Implementation-of-Video-Compression-H.264
Implementation of video encoder/decoder using MATLAB

My Project of the Information Theory and Coding Course Offered in Fall 2022 @ Zewail City.

In this project, I implemented the Viterbi Decoder and compared the results with the MATLAB Built-in function of Viterbi Decoder.


Given a Convolutional an encoder for a rate r = 1⁄2, constraint length K = 4 convolutional code. 
Starting with the all-zero state, and the received sequence is 111101011010... 
Using the Viterbi algorithm, compute the decoded sequence.


## Implementation Steps:

A) Viterbi Decoder 

            1) In order to design a Viterbi code for the encoded message, the Generative polynomials are needed.
            2) g = [1 1 1 1 ; 1 1 0 1] based on the below figure.
            3) After that, the table with path metric is constructed.
            4) The table is filled based on the hamming distances.
            ![image](https://user-images.githubusercontent.com/58476343/220167431-d1d11541-de7c-432e-9082-470194f8e28b.png)
            5) Finally, the backward bits identification is performed to find the exact decoded message.
            ![image](https://user-images.githubusercontent.com/58476343/220167457-43ecc05e-b898-4588-a6e3-926598616e5c.png)


## HIGH Compression Video <a name="HIGH Compression Video"></a>
https://user-images.githubusercontent.com/58476343/220160074-7c0bb5df-cd9f-46c6-8ec2-78530db7aad6.mp4
