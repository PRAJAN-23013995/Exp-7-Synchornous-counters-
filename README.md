![WhatsApp Image 2023-12-14 at 20 27 33_d5d21625](https://github.com/PRAJAN-23013995/Exp-7-Synchornous-counters-/assets/150313345/4d864ee7-a8ee-4422-8594-b047cedf0d47)![WhatsApp Image 2023-12-14 at 20 27 33_d5d21625](https://github.com/PRAJAN-23013995/Exp-7-Synchornous-counters-/assets/150313345/fc4dad44-18ed-47b6-a6d4-e6a2635243b3)# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)
![WhatsApp Image 2023-12-14 at 20 27 33_436abc51](https://github.com/PRAJAN-23013995/Exp-7-Synchornous-counters-/assets/150313345/8ed65f04-8845-4937-9f3f-963f6f7c9b1c)

![WhatsApp Image 2023-12-14 at 20 27 32_b0baeda1](https://github.com/PRAJAN-23013995/Exp-7-Synchornous-counters-/assets/150313345/6a19f649-c65e-41bf-baa4-099c7c59a4d6)


## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.

![WhatsApp Image 2023-12-14 at 20 27 33_f17fb146](https://github.com/PRAJAN-23013995/Exp-7-Synchornous-counters-/assets/150313345/024acb33-96c2-453a-9c1b-594f1d56191c)
![WhatsApp Image 2023-12-14 at 20 27 34_13aff570](https://github.com/PRAJAN-23013995/Exp-7-Synchornous-counters-/assets/150313345/7b07388c-4a96-4d55-8ada-34047cacc918)
![WhatsApp Image 2023-12-14 at 20 27 33_d5d21625](https://github.com/PRAJAN-23013995/Exp-7-Synchornous-counters-/assets/150313345/baed7f9f-394e-4cc3-98d7-16b6808f9e79)

4-bit Count Down Counter
### Procedure
/* write all the steps invloved */


### PROGRAM 
/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: 
RegisterNumber:  
*/





### RTL LOGIC UP COUNTER AND DOWN COUNTER  









### TIMING DIGRAMS FOR COUNTER  





### TRUTH TABLE 


![download](https://github.com/PRAJAN-23013995/Exp-7-Synchornous-counters-/assets/150313345/895c4e19-7320-47a7-9f45-301421febea7)
![download](https://github.com/PRAJAN-23013995/Exp-7-Synchornous-counters-/assets/150313345/895c4e19-7320-47a7-9f45-301421febea7)






### RESULTS 
