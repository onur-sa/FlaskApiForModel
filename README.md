# FlaskApi
Graduation Thesis of Data Analytics of IOT (2019)

Face Recognition With Cloud Computing

This project is a facial recognition prediction project with an android application. The project consists of 3 parts: Android application, Recognition model and Flask API. Briefly, the project works like this: We send a face photo taken with the Android application to the Flask API, where the Recognition Model is installed, via the ngrok tunnel. Then the Flask API sends a response to the Android application. And we see this response on the screen.

I am proud to say that this project is done by me Onur Saldamlı and my team mate Ezgi Eftekin and is our graduation thesis.
First of all, we did the necessary pre-processes and authentication processes to create the Flask API.
Previously, we created our model and saved it as model.h5. Now we need to send the photos we have taken from our android application to this Flask API and get a response.

About Code :
We use two different functions for this. With the cnn() function, we load the model and label the results.
Then, with the for loop we created, we transform each photo into a form that the model can understand. (grayscaling, resizing, etc.)
Finally, we rotate the label.
Currently, when a photo is uploaded to the model, the model can create a result.
But we need to write a function to send photos and get return, we create the upload_photo() function for this.
With this function, the output is transferred to an ngrok URL and the android app takes this output from there.
