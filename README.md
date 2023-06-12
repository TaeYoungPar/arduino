# arduino Annyoing Alarm Clock
# https://www.instagram.com/p/CdaVRpSOylp/     

Project information 
Sometimes we overslept because we don't hear our alarm in the morning. If this situation repeats, we may not be able to do what we planned or have other negative effects. Conventional alarm clock wakes people up with sound. However, sometimes we did not hear the sound and keep sleeping. We planned this project to solve this situation. Our project is to have the webcam recognize the face when the alarm goes off and spray water on it. This will help people who have difficulty waking up in the morning. Even if someone who does not hear the alarm, it will wake you up with enough stimulation to spray water.
Progress by development schedule 
Our previous plans are as follows:
- Prepare programs and materials to be used in the project by March 20. (Webcam, OpenCV, Python, motor, button, etc.)
-	Create an alarm clock that is the basis of the project by March 27th.
-	Create face tracking function through OpenCV by April 6th
-	Combine alarm clock and water spray function by April 13th
-	Combine the face tracking function by April 20 and test if all functions are working
-	Combine the face tracking into existing projects by April 20
-	Testing and Debugging Projects Before Presentation

We followed this plan as closely as possible. However, as the semester became busier, sufficient testing and debugging did not proceed. Also, every time we tested, different errors occurred, and it took a long time to solve them. In the end, we didn't quite follow the plan, but fortunately our results were successful.

What you have completed (difficulties/solutions)
We encountered a variety of errors and problems frequently, but our project worked as we had planned. First, we implemented the alarm clock. In order to implement the alarm clock we need RTC which always stored time and three buttons were needed for setting the time and alarm time. Basically, I had the necessary materials to make an alarm clock, but it was difficult to obtain RTC. We placed an order on Amazon, but they lost our package twice, so we didn't test the alarm clock until we received the item. We were able to set the alarm clock without RTC, but if the power connection was lost, the data set disappeared. However, as a result of waiting for 3 weeks, we were able to get an RTC and the alarm clock worked properly. Second, face tracking through webcam was implemented. Using the face tracking library provided by OpenCV, the web cam recognizes faces by using python and Arduino at the same time. We used two servo motors to make the web cam move along the x-axis and y-axis to track the face. Finally, it was to operate the sprayer, which was the most difficult. The handle of the sprayer should be pulled using two servo motors, but in this process, the servomotor was weak and could not be pulled sufficiently. To solve this, we used a variety of sprays. The handle of the first sprayer was not smooth enough, so it did not trigger. In the second attempt, a water gun was used instead of a sprayer, and the handle was pulled enough, but the water gun itself was problematic and could not shoot water. In the third attempt, a smooth handle was used, but the spray was too large and could not be combined with the web cam. In the last attempt, we got a small spray, and we finally succeeded using a smooth handle. These three different physical and programmatic combinations were combined, and everything worked well. However, we think it would have been better if the motor could produce a little more output on the sprayer.


Reasons why it misses from the proposed plan 
We have not missed anything in particular, but we are lacking in our project. The servo motors in our spray were too weak for what we thought. That is why the handle could not be pulled completely. We think we would have had better results if we used different motors. However, it can still spray water through the two servo motors, and it will make you wet enough.
Project future plan
This project of version 1 has various shortcomings. First, these are not organized neatly, so it is distracting to see. In other words, it is not fancy. We need to make a cover using a box or 3D printer to make it more commercial. Also, we can make it more fancy by using the touchpad instead of the buttons. Second, there is insufficient power. It requires a lot of power to use a total of 4 motors and the configuration of the digital alarm clock. Provide sufficient power to the project using additional high external power. Finally, we need a webcam to use this, which must always be connected to a laptop. If the webcam can be run on the Arduino itself without connecting it to a laptop, it will be a wire-free project. In other words, the spatial limitation will disappear. we think it would be a product that would be commercial enough if all of these were available in version 2.
