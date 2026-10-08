# Improve the Accuracy of Satellite Navigation Systems

## MathWorks Capstone Project - Project ID 192

This repository contains the MATLAB implementation of the MathWorks Capstone Project **"Improve the Accuracy of Satellite Navigation Systems"**.

The project focuses on improving the reliability of satellite navigation communication at low Signal-to-Noise Ratio (SNR) using **non-binary LDPC coding** for **BeiDou navigation messages**.

## Objective

The main objective of this project is to improve the accuracy and reliability of satellite navigation messages by using non-binary LDPC error-correcting codes and evaluating their performance under noisy communication conditions.

## Technologies Used

- MATLAB
- Non-Binary LDPC Coding
- GF(64) Finite Field
- BPSK Modulation
- AWGN Channel
- BER Analysis
- BeiDou Navigation Message Structure

## Project Workflow

The implemented system follows these steps:

1. Generate a 288-bit BeiDou navigation message.
2. Convert the binary message into GF(64) symbols.
3. Encode the message using a non-binary LDPC encoder.
4. Perform BPSK modulation.
5. Add AWGN noise at different SNR levels.
6. Decode the received data using the LDPC decoder.
7. Convert the decoded GF(64) symbols back into binary bits.
8. Calculate the Bit Error Rate (BER).
9. Plot and analyze BER performance for different SNR values.

## Repository Structure

```text
Improve-Satellite-Navigation-Systems/
│
├── 01_MathWorks_Project/
│   └── Project_192_Description.pdf
│
├── 02_BeiDou_ICD/
│   └── BeiDou_ICD.pdf
│
├── 03_MATLAB_Code/
│   ├── main.m
│   ├── createNavigationMessage.m
│   ├── bitsToGF64.m
│   ├── gf64ToBits.m
│   ├── ldpc64Encoder.m
│   ├── ldpc64Decoder.m
│   ├── addAWGN.m
│   ├── calculateBER.m
│   └── plotResults.m
│
├── 04_Data/
│   ├── H_matrix.mat
│   ├── reference_message.mat
│   └── reference_encoded.mat
│
├── 05_Results/
│   ├── BER_Result.mat
│   ├── BER_Table.xlsx
│   ├── BER_vs_SNR.png
│   ├── Original_Message.png
│   ├── BPSK_Signal.png
│   └── Received_Signal.png
│
├── 06_Report/
│   └── Project_Report.pdf
│
└── README.md
