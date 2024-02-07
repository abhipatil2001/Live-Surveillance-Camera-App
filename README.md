1. PROPOSED SYSTEM : 

In this proposed system the user can use old smart phones which contains camera and start the
system by Pairing with QR code or by Pin, when the smart phone is paired with another
smartphone the user can see live feeds from old smartphone.
The live video is captured and saved in secondary storage System, the user can view live feeds
from another camera and can get notified if there are any changes in system. In this proposed
work we have added new features where the user can interact by Two-way talk through
microphone and can send required message through old smart phone.
There are various functions embedded in this system such as the user can keep an eye on with
what he/she care about at anytime from anywhere; just like a security camera. The user can get
instant notification when the Camera picks up on any movement. There is a function of Two
way talk you can deter thieves, interact with visitors or pets, and soothe babies. There is also a
low Dark mode with low light feature where the user can save battery and can detect the person
in dark also it can work in background. The siren can be used to Scare away intruders, protect
your possessions even when you are far away from the house. Person Detection Mode allows
user to avoid unwanted alerts triggered by irrelevant objects in your environment.
The new feature added in thissystem is community where we can use it as a chatting application
when the user is far away from the home town, he/she can give alert and notify persons in
community in fraction of seconds through custom messages.
The proposed system also gives a user cloud storage where the live feeds can be stored without
any hardware storage and can manage the storage by paying small amount.

2	Interface : 

The interfaces are a central part of android development application whereby shows the flow of interfaces on an application.

2.1	Registration module : 
The registration process for our system is designed to ensure the security and privacy of user accounts. Users can access the registration page by visiting the system's homepage and clicking on the "register" button. 
They will then be prompted to enter their email address, phone number, and a password.

![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/316eef6a-1cc8-4b0c-ab1a-6ee44a572fac)


2.2 QR code Generator Module:

To implement a QR code generator in our Android application, we used the ZXing
(Zebra Crossing) library, which is an open-source library for generating and reading
QR codes. We created a new Activity or Fragment to handle the QR code generation,
and added a button or other control to initiate the process. When the user clicks this
button, we used the MultiFormatWriter class from the ZXing library to create a QR
code image using the encode method and the desired QR code format (such as
QR_CODE). This returned a BitMatrix object, which represents the QR code image.
We then used the BitMatrixToImageWriter class from the ZXing library to convert the
BitMatrix to a BufferedImage and displayed the image in an ImageView using the
setImageBitmap method. Optionally, we also provided a way for the user to save or
share the QR code image by adding a save or share button and using the Android file
system or sharing API to save or share the image.
The detail steps are given below:
1. Add the necessary dependencies to your project's build.gradle file. You will need to
include the ZXing (Zebra Crossing) library, which is an open-source library for
generating and reading QR codes.
2. Create a new Activity or Fragment to handle the QR code generation. This is where
you will build the user interface and implement the code to generate the QR code.
3. Add a button or other control to initiate the QR code generation. When the user clicks
this button, you will create a QR code image using the ZXing library and display it in
an ImageView.
4. To create the QR code, you will need to use the MultiFormatWriter class from the
ZXing library and call the encode method, passing in the data that you want to encode
and the desired QR code format (such as QR_CODE). This will return a BitMatrix
object, which represents the QR code image.
5. To display the QR code image in the ImageView, you can use the
BitMatrixToImageWriter class from the ZXing library to convert the BitMatrix to a
BufferedImage, and then display the BufferedImage in the ImageView using the
setImageBitmap method.
6. Optionally, you may also want to provide a way for the user to save the QR code
image to their device or share it with others. You can do this by adding a save or share
button and using the Android file system or sharing API to save or share the image.


![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/481954b0-4cf1-40e3-a503-62db96e773f5) ![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/655fb3f9-a006-4e9e-8411-da96ae6520e6)

2.3	Scanning QR for pairing : 


![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/d74dcf3a-9369-4174-8e7c-d08711deefb0)  ![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/4a0a5aa7-c627-46b8-a4c1-233f40a81b88)

2.4	Camera recording interface :


![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/fef264ac-f5dc-4f46-94ba-2583a41e1c3c)

After pairing the camera using QR code we generate the screen where we can see the live
records in camera mode, when “CAPTURE” button is pressed we display the following screen
where live recording is captured to store the recording. We can use the “STOP” button to stop
recording the content and hence we can exit through the application.

2.5 Uploading interface :

![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/9baafc83-3b6a-4a0d-ba32-adf087da59a2)

Now when the recording is captured we have given the storage to upload the files to google cloud and internal storage this can be done when the whole uploading process is finished and when the message popup “Upload finished”, the uploading process is completed.

2.6	Motion detection through camera : 


![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/0ee64927-a990-423f-acbd-d570cd5059e3)   
![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/5cf05540-d3d8-449a-8c66-bdc8d2c23cc6)

When the video is captured by camera the motion detection algorithm plays an important role, it shows the red coloured spot on the motion of the object. The figure above illustrates the same behaviour of the object and whenever such detection takes place the instant notification is send to the user. By implementing this concept in this application we can get alert provided the user is in the motion.

2.7  Internal storage module 

![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/d1af001c-bfd1-4174-9e2e-8eb91a837af6)

This module shows the stored recording of the application this can be seen in the android mobile where the path through the mobile is given.

2.8  Cloud storage module  

![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/aede95bf-ef33-4941-8806-c550526baf3c)

This is the cloud storage module where the recording is stored parallelly in the cloud. Here we have used google drive this can be used for cloud storage we can also integrate this storage system through another cloud services.

2.9  Community Registration module : 

![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/864b9b98-7898-4ead-9b9c-79326b8cec54)  ![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/e606a02a-df97-4148-861f-2b5366febf9d)

To be a part of community where we can send alert to the registered people and also to the neighbour, the community registration is mandatory. To register the people to community they should click on three dots on top left corner to open the drawer, in the drawer there is the option for “Add Community” as displayed in the Figure 2.10, the registration form appears the user should fill the necessary information and submit the form by clicking in “ADD TO COMMUNITY” as should in Figure 5.2.10.

2.10  Community Alert module :

![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/4a5682e3-691c-4019-874a-d95d0325e1c1)

This is the next step after registering to community. The screen is displayed as shown in Figure
2.9 where the user should only press the “SEND TO ALL” button to send the alert in form of text message in the community. When an user needs to send alert message to individual person then they can send individually through “Send” button shown above. By default message the alert message is set as “Danger Alert”, we can modify or can customize the message by typing the message on the textbox. We can give alert through this method


3. SYSTEM ARCHITECTURE :

In the system architecture, the flow of the system is organized to enable the system development will progress smoothly and efficiency. The way of the system functioning is drawn in the diagram to make clear understanding of each process of the system during the development phase.


![image](https://github.com/abhipatil2001/Live-Surveillance-Camera-App/assets/115881224/dd13b969-95e4-4063-8165-b7e6db768400)


HERE THE SYSTEM IS INTEGRATED WITH GOOGLE DRIVE AS A CLOUD STORAGE. INTEGRATING APPLICATION WITH ENTERPRISE CLOUD PLATFORM IS IN FUTURE SCOPE


4. CONCLUSION :
   
In conclusion, video surveillance cameras have become increasingly popular as a security measure for homes and businesses. By using an Android device as a surveillance camera, users can easily monitor their properties remotely and receive notifications of any activity. The implementation of a video surveillance camera using Android involves setting up a camera, connecting it to the internet, and using an app to access and control the camera remotely. While there are many options available for Android-based video surveillance cameras, it is important to carefully consider the features and capabilities of each option in order to choose the best solution for the specific needs of the user. Overall, the use of an Android device as a video surveillance camera provides a convenient and cost-effective way to enhance security and protect against potential threats.
In addition, the use of Android allows for a wide range of customization and integration with other security systems, such as access control and alarm systems. Overall, the implementation of a video surveillance camera using Android can provide a cost-effective and convenient solution for monitoring and protecting people, property, and assets.
