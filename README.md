# PID_udacity


#### Effect of propotional term 

The main use of the propotional term is to determine the strength of the correcting value (steering,throttle , break) based on the error . if the error is large then the correctig value is large and vice versa . if the P value is high , the correction force applied to the system will also be high . this will caluse the system to overshoot beyond the desired goal .

#### Effect of integral term 

This term will use the overall error occured during the process . according to the error intensity this term will shoot control valuse (steering , throttle,break) to move the system close to the desired goal . the main use of this term is when the system takes long time to achieve the goal (i.e it goes parallel to the central line (goal) for a long time )

#### Effect of differential term

The concept here is , if the last command we send to correct the system actually increased the error , then we need to pull back the correction value . imagine if we send a cmd and it drives the system beyond the goal line , the difference between the previous error and the current error increases . the derivation term makes use of this to pull back the command value we send to slow down the rate at which we approach the goal . this value actually slows down the system mainly when the system goes passed the goal line and brings the system back by sending negative values 

#### how i derived the final PID values

I used trial and error method because the twiddle method cannot be used here .

* NOTE : it will be helpful if you can guide me on how to find the value for PID without trial and error method or a good way to find the values ...
