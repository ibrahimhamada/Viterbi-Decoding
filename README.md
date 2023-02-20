# Implementation-of-Viterbi-Decoding

# Implementation-of-Video-Compression-H.264
Implementation of video encoder/decoder using MATLAB

My Project of the Information Theory and Coding Course Offered in Fall 2022 @ Zewail City.

In this project, I implemented the Viterbi Decoder and compared the results with the MATLAB Built-in function of Viterbi Decoder.


Given a Convolutional an encoder for a rate r = 1⁄2, constraint length K = 4 convolutional code. 
Starting with the all-zero state, and the received sequence is 111101011010... 
Using the Viterbi algorithm, compute the decoded sequence.

## Convolutional Enoder Diagram  <a name="Convolutional Enoder Diagram"></a>
![image](https://user-images.githubusercontent.com/58476343/220167431-d1d11541-de7c-432e-9082-470194f8e28b.png)

## Possible States with inputs and outputs  <a name="Possible States with inputs and outputs"></a>
![image](https://user-images.githubusercontent.com/58476343/220167457-43ecc05e-b898-4588-a6e3-926598616e5c.png)

## Implementation Steps:

A) Viterbi Decoder 

            1) In order to design a Viterbi code for the encoded message, the Generative polynomials are needed.
            2) g = [1 1 1 1 ; 1 1 0 1] based on the below figure.
            3) After that, the table with path metric is constructed.
            4) The table is filled based on the hamming distances.
            5) Finally, the backward bits identification is performed to find the exact decoded message.
            

B) MATLAB Viterbi

            1) In this part, I used the built in function to confirm the obtained results.
            2) poly2trellis() function is used to find the trellis.
            3) Constraint Length K = 4
            4) CodeGenerator = [17 15] which is equivalent to [1111, 1101] in octal.
            5) vitdec() is used to decode the message using the constructed trellis.
            6) 'trunc' — Specifies truncated operating mode.
            7) 'hard' — The decoder expects binary input values of 0 or 1.
            
