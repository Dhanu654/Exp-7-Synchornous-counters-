# Exp-6-Synchornous-counters - up counter and down counter 
### AIM:
To implement 4 bit up and down counters and validate  functionality.
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



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![image](https://user-images.githubusercontent.com/36288975/169644844-1a14e123-7228-4ed8-81a9-eb937dff4ac8.png)


4-bit Count Down Counter
### Procedure
![image](https://github.com/Dhanu654/Exp-7-Synchornous-counters-/assets/148514965/f246bbe0-2a90-454a-8fd7-49a70e5912b3)




### PROGRAM:
/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.
~~~
Developed by: Dhanusya.K
~~~
RegisterNumber:  23006651
# UP COUNTER:
![image](https://github.com/Dhanu654/Exp-7-Synchornous-counters-/assets/148514965/917296af-d2c5-40d6-aa3f-73d5df29b4de)
# DOWN COUNTER:
![image](https://github.com/Dhanu654/Exp-7-Synchornous-counters-/assets/148514965/6341fdad-cd02-429c-873e-402f30e01526)

*/






### RTL LOGIC UP COUNTER AND DOWN COUNTER
# UP COUNTER:
![Screenshot 2024-01-03 082001](https://github.com/Dhanu654/Exp-7-Synchornous-counters-/assets/148514965/e2232092-e1e5-4110-8e68-c5a79f7bde82)
# DOWN COUNTER:
![Screenshot 2024-01-03 081729](https://github.com/Dhanu654/Exp-7-Synchornous-counters-/assets/148514965/ae9e9b41-0049-4dec-a195-e07af56aceff)

### TIMING DIGRAMS FOR COUNTER  
# UP COUNTER:
![Screenshot 2024-01-03 081854](https://github.com/Dhanu654/Exp-7-Synchornous-counters-/assets/148514965/74d55e68-5cf0-460d-9929-19dcb8c3f87f)
# DOWN COUNTER:
![Screenshot 2024-01-03 081835](https://github.com/Dhanu654/Exp-7-Synchornous-counters-/assets/148514965/ff148765-4d85-45f9-87cd-258b7f03e6fc)


### TRUTH TABLE 
# UP COUNTER:
![Screenshot 2024-01-03 100540](https://github.com/Dhanu654/Exp-7-Synchornous-counters-/assets/148514965/c1742038-5ac5-4a1a-8476-7800d0b2a236)

# DOWN COUNTER:
![Screenshot 2024-01-03 100601](https://github.com/Dhanu654/Exp-7-Synchornous-counters-/assets/148514965/0c336fc8-d9b1-4166-98d2-84d0b03309fc)




### RESULTS 
Thus the Program executed Successfully
