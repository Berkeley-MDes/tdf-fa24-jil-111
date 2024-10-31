# Week8  Reflection #
### Week of 10/31/2024



# Week  Reflection #
### Week of 10/24/2024



# Week 7 Reflection #
### Week of 10/17/2024

# Week 6 Reflection #
### Week of 10/10/2024

I work on thinking about the project and write the project proposal. The following diagrams are what our project look like and the system we build. 

![Alt text](assets/wishing.png)
![Alt text](assets/wishingdiagram.png)

## Reflections
Through the development of the "Whispers of Wishes" project, we learned several important lessons about the integration of physical components and cloud-based services. One key takeaway was the significance of calibration in force sensors; ensuring they respond accurately to varying degrees of pressure required precise coding and adjustment of sensitivity. This process not only deepened our understanding of sensor technology but also emphasized the need for iterative testing in prototyping.

Another important aspect was learning how to optimize cloud connectivity between Photon2 and Particle Cloud Services. Although cloud communication is vital for remote interaction, we encountered occasional latency and instability issues. Troubleshooting this problem required us to dive deeper into Wi-Fi management, leading to the realization that network stability is a critical factor in real-time interactive installations. Overall, these challenges have pushed us to explore new solutions and highlighted the complexity of integrating hardware with cloud-based systems in a cohesive and seamless manner.

Currently, the project is in the early stages of prototyping. The basic components—force sensors, LEDs, and the servo—have been successfully integrated, but further refinement is required, particularly in terms of response time and mechanical precision. While the system functions, it is clear that more fine-tuning is needed to enhance user interaction and create a smoother, more immersive experience.

## Speculations
Looking ahead, there are several promising directions for the evolution of this project. First, we plan to explore more sophisticated user interactions by incorporating additional sensors, such as proximity or sound sensors, to create more dynamic and personalized feedback loops. For instance, the sound of coins hitting the wishing fountain could trigger different LED patterns or movements, adding another layer of engagement for users.

Another future direction involves improving the power efficiency of the system, particularly if we want to deploy this installation in an outdoor setting. Investigating solar-powered solutions or low-power modes for the Photon2 and its connected components could significantly enhance the longevity of the project. Additionally, integrating machine learning algorithms to adapt the system's responses based on user input patterns could make the experience more interactive and personalized over time.



# Week 5 Reflection #
### Week of 10/02/2024

## 01 Compiled and flashed successfully for 01_hellworld


When I first created the project and tried to compile it. Errors occur. 

![Alt text](assets/helloworlderror.png)

So I asked ChatGPT how to solve this problem and it really helped me. I realized that I need to clean the project. Sometimes, cached files in the build environment can cause issues. So I tried cleaning the project:open the command palette by pressing ⇧⌘P (macOS); Type Particle: Clean Application for Device and select it. This removed any cached build files that might be causing the error. This method really helped me cleaning the cached files and I successfully compiled the file at the end. 
![Alt text](assets/helloworldsucc.png)

After I compiled the file, Photon2 successfully flashed. I also opened the Serial Monitor: open the command palette (⇧⌘P on macOS) and type Particle: Serial Monitor. This opened a terminal window where I can saw the output from my Photon 2. Every 3 seconds, I saw the following messages:
Hello World!
the number of characters in that msg was 12.
![Alt text](assets/helloworldflash.png)

## 02 Compiled and flashed successfully for 02_helloworld_spell

After the first try, I continued to compile and flashed the next two files that Jeff shared. And one thing I think is important is to choose the device at the bottom of the page each time creating a new file. I forgot about this for the second time and was not able to compile and flash. 

![Alt text](assets/spellcompile.png)
![Alt text](assets/spellflash.png)

## 03 Compiled and flashed successfully for 03_altering_periodicity

The following two images show how I compiled and flashed Photon2 successfully. I followed the steps I took earlier and didn't encounter any issues. 

![Alt text](assets/alterPeriodCompile.png)
![Alt text](assets/alterPeriodflash.png)

Over the course of these three practices, I have learned the essential workflow for developing and deploying firmware to the Photon 2 microcontroller using Particle Workbench. This process involved setting up the development environment, writing basic C++ code, compiling it successfully, and flashing the firmware to the Photon 2 device. I encountered and resolved several challenges, such as device compatibility issues and platform mismatches, which enhanced my understanding of the importance of correctly configuring both the target device and the operating system within the development environment.

Through multiple errors, such as compilation failures and device flashing mismatches, I learned to troubleshoot effectively. The key takeaway here is ensuring that both the correct device and OS version are selected, as seen when the project initially targeted an Argon device instead of Photon 2. 

I gained a deeper understanding of how the Serial LogHandler functions, enabling me to debug by logging real-time messages to the Serial Monitor. This functionality is vital for monitoring the behavior of firmware in action, particularly when working with sensor data or debugging loops.

I primarily learned by doing, following the step-by-step process of copying, pasting, and modifying code provided by Jeff. Each practice session built on the last, introducing new concepts and challenges, which I had to troubleshoot and resolve on my own or with guidance. The hands-on, iterative nature of this process allowed me to become familiar with Particle Workbench and the Photon 2 microcontroller's capabilities.

## 04 button -> led pulse rate

![Alt text](assets/buttonLEDpulse.png)
![Alt text](assets/lighton.JPG)

For this practice, I first compiled the file. And then tried flashing it. The problem I encountered is the light is not flashing when I press the button, it only turns green. And after few minutes, the light is off. So I started to check how I conncet the breadboard, and I saw my button conncections and light conncections are wrong. I connect the bottom-right leg of the button to pin D10 instead of D6, and connect a lead from this middle rail to USB on my Photon 2 via the associated middle rail instead of D6. I encountered this issue because I was only estimating from the image that Jeff provided, and tried conncecting to the same spot without looking at if it is D6 or D7. After looking carefully at the file again, I corrected my the erros and was able to control the flash rate by pressing the button. 


Moving forward, there are several areas that I believe will be critical to explore:

1. Understand how code works and how it is connected to the breadboard.
2. Be more familliar with how the conncections on breadboard work. It is easy to follow the iamges, but it is difficult to do a project without these images to follow. So I think it would be important for me to explore different parts of Photon mean and how these parts could be controlled over codes.




# Week 1 Reflection #
### Week of 09/05/2024

## 1. Design in Tech 2017 Report Video

This week, I watched the Design in Tech Report Video because I am curious about our first project. This video briefly 
introduces what computational design is and why we need this. While watching this video, I would randomly put some key words on my notebook to get myself focused since it is a long video. 
![Alt text](assets/Hand-writtenNotes.JPG)
Specifically, in my screenshots below, it highlights the design
education biases back in 2017, which gives me some thinking about the design frameworks that I have been following in the past, which is the use of empathy. It is interesting to see how using empathy to design was a Top 2 educational biases back then. The limit of empathy should be emphasized in many of my designs. 
![Alt text](assets/Tech-Report-Screenshot)

In order to explore how to deal with limit of empathy, I read an article [The Promise of Empathy](https://creativetech.mat.ucsb.edu/readings/promise_of_empathy.pdf): Design, Disability, and Knowing the “Other" by Bennett, C. L., & Rosner, D. K, in which the authors advocates "ongoing attunement, which is a continuous harmonization with the users’ evolving experiences and perspectives." It dawned on me that genuine empathy required more than just stepping into someone's shoes; it necessitated inviting them to walk the path with me. This is why user research and design are interative process because the evaluations of our products are made by our users. Therefore, after designing my own physical products, I think it is important for me to invite students in our cohort to evalaute it. 


## 2. Using 3D Printer

I also imported the 3D models I downloaded from the internet to Cura. I followed the instructions and successfully 3D printing the obejcts. In the following week, I will start to explore whether Maya could be imported to Cura or other useful software tools. I have also started Rhino Tutorial and am excited to learn more about Grasshopper as well. This week I will explore more aspects about computational design from papers and videos online to be more specific about my first project. 

![Alt text](assets/Weekone-Cura)
---
# Week 2 Reflection #
### Week of 09/12/2024

## 1. Basics on Rhino

In the workshop of the Tuesady's class, I went over the basics of Rhino. For example, how to create the squares, the curve lines. ![Alt text](assets/BasicsRhino.png) It is interesting that everything on Rhino is based on the command line, which I was not very familiar with. 

## 2. Basics on Grasshopper

### Grasshopper Tutorial 01
I followed a youtube video to get started with Grasshopper because I am still confused about many components in the PhoneStand file. I think I would need some time to get familiar with Grasshopper more by starting to create some simple things first. In the tutorial 1, I have learned how to move a sphere using Grasshopper by connecting Geom Component with sphere on Rhino -> adding Move Component -> adding number Slider to control the range of movement.
![Alt text](assets/GrassMove)

The link for the tutorial is here (https://www.youtube.com/watch?v=your_video_id)

### Grasshopper Tutorial 02 Dividing Curves
I followed the youtube video I emntioned earlier and learned three differnent components to divide a curve. I took notes of the logic of using these components.

1. Divide Curve
   - Input: C-curve; N-Number of segements in this curve(use number slider to define by myself)
   - Output1(Curve): P-Shatter Component(we need indivisual segment of the curve); Shatter has 't' as a value to represent a point in the curve(we need to link the input 't' in Shatter with output 't' in Divide Line.
  ![Alt text](assets/divideCurve.png)
   - Output2(PolyLine): Use PoliLine Component to divide the curve into straightline. Hit Option+Space to bake the line in Rhino. 
  ![Alt text](assets/divideCurvToLine.png)
   - Divide Curve component already breaks the curve into a series of points; however, it does not actually split the curve into segments or pieces. Instead, Divide Curve only provides points along the curve at specified intervals but does not alter the curve itself.
2. Divide Distance
   - Input: C-curve; D-Distance we define
   - Output: PolineLine Component
  ![Alt text](assets/weektwoDiDist.png)
3. Divide Length
   - Input: C-curve; L-Length we define
   - Output: PolineLine Component
   ![Alt text](assets/twoCurveDistance.png)


# Week 3 Reflection #
### Week of 09/19/2024
### Grasshopper Tutorial 03 Dividing Surfaces
1. Divide Domain
   - Steps: In Rhino, Create a curve and in Command line "Extrude curve" to create the surface
   - Input: Domain-Surface; U count and V count- Number Slider;
   - Output: IsoTrim to divide the the surfaces
  ![Alt text](assets/isotrimSurface.png)
2. Divide Curve
   - Overall Logics
     a. Divide a curve into points.
     b. Use the Shatter to break the curve into segments based on the points.
     c. Extrude each curve segment along the Z-axis to give the segments a 3D height.
     d. Apply a Linear Array to duplicate the geometry along a given direction.
     ![Alt text](assets/DivCurv.png)
![Alt text](assets/divCurveSurface.png)

### Project for the Class(Bracelet Holder)

![Alt text](assets/slide1.png)
![Alt text](assets/slide2.png)
![Alt text](assets/slide3.png)
![Alt text](assets/slide4.png)
![Alt text](assets/slide5.png)
![Alt text](assets/slide6.png)
![Alt text](assets/slide7.png)
![Alt text](assets/slide8.png)
![Alt text](assets/slide9.png)
![Alt text](assets/slide10.png)
![Alt text](assets/slide11.png)

![Alt text](assets/workflow.png)
### Another project on Phone stand
I tried to created the phone stand on my own, using the logic of points-curves-surface-solid. The process is very time-consuming and I encountered problems such as how to close the surface, how to transforms the surface into solid... With the help Chat GPT and classmates, I was able to generate the right phone stand I want. I used SetSurface in Rhino to transform the surface into 3D models that is printable. 

![Alt text](assets/phoenstan1.png)
![Alt text](assets/phoenstand2.png)
![Alt text](assets/phonestand.png)


# Week 4 Reflection #
### Week of 09/26/2024

![Alt text](assets/conceptMap.png)

This map illustrates the Personal Device Ecosystem that I interact with daily. At the center is my smartphone, which syncs data with various devices and services. My laptop and tablet sync with the phone through cloud platforms like iCloud , ensuring that files, messages, and calendar events are shared across devices. Feedback loops are created when notifications from my laptop (e.g., new email) are pushed to my smartphone, prompting further actions.

#### Key Components in the Ecosystem
Smartphone (central device that syncs with other devices and services)

Laptop/Tablet (another device syncing with the smartphone through cloud services)

Cloud Storage Services (iCloud)
Connectivity (Wi-Fi, Bluetooth) to facilitate data syncing

#### Information Flow
Messages: Syncing between phone and cloud services to ensure I can see messages on all devices.

Files/Photos: Data synced between my phone, cloud storage (iCloud), and accessible on other devices like a laptop.

Reminders/Calendar: Calendar events created on my laptop sync to my phone via the cloud.

#### Map Out the Information Flow and Feedback Loops
Smartphone ↔ Cloud Storage (iCloud): Files, photos, and messages are synced between the phone and the cloud, ensuring they are backed up and accessible on other devices.

Smartphone ↔ Laptop/Tablet: The phone syncs messages, calendar events, and other data via cloud services, allowing the laptop to access the same data.

Feedback Loop: Notifications from apps (e.g., new email on laptop, reminder from calendar) trigger feedback on the phone, such as alerts.

### Thoughts
By creating a map, I am identifying how various systems, platforms, and devices connect and interact with one another in my daily life. I analyzed how data flows between them and where feedback loops exist. My second project involves designing a digital ecosystem where different components like sensors, microcontrollers, and cloud services interact with each other. The mapping exercise helps me think about the various elements that interact in a system and how they influence one another, which is crucial when developing my own ecosystem.

This mapping skill will transfer directly to my project, where I'll need to map out how data is collected (e.g., sensors), processed (e.g., Photon 2 microcontroller), transmitted (e.g., cloud services), and fed back to the user. I'll be working with data flow and feedback loops constantly in my digital ecosystem design.




