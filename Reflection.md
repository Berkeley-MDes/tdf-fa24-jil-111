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


# Week 3 Reflection #
### Week of 09/26/2024






     

