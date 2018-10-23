# Video Doorbell, Lab 7

*A lab report by Matthew Dalton*

### In This Report

1. Upload a video of your version of the camera lab to your lab Github repository
1. As usual, update your class Hub repository to add your [forked IDD-Fa18-Lab7](/FAR-Lab/IDD-Fa18-Lab7) repository.
1. Answer the questions in-line below on your README.md.

## Part A. HelloYou from the Raspberry Pi

**a. Link to a video of your HelloYou sketch running.**

https://youtu.be/IDf51CL-kF0

## Part B. Web Camera

**a. Compare `helloYou/server.js` and `IDD-Fa18-Lab7/pictureServer.js`. What elements had to be added or changed to enable the web camera? (Hint: It might be good to know that there is a UNIX command called `diff` that compares files.)**

To enable the web camera, we just have to add the line:

```socket.emit('takePicture');```

to the function takePicture in the client.js file.

**b. Include a video of your working video doorbell**

https://youtu.be/8gfoqtx7cH0

## Part C. Make it your own

**a. Find, install, and try out a node-based library and try to incorporate into your lab. Document your successes and failures (totally okay!) for your writeup. This will help others in class figure out cool new tools and capabilities.**

For part C I used the emailjs library to send myself an email with a copy of the picture taken by the video doorbell. The key insight that allowed me to use this package was realizing that I had to create a dummy email for the pi to connect to the gmail server to send my picture. The changes I made using this library can be found in the pictureServer.js file. 

**b. Upload a video of your working modified project**

https://youtu.be/axmpJlWl7P8
