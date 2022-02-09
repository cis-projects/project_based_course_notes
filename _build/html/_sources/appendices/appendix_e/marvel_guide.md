# Marvel Tutorial
This tutorial shows you how you can use Marvel to help you create your paper prototype. 

## Before You Start Prototyping

Before you start prototyping, let us remind ourselves - why are we creating paper prototypes?  What's the purpose 
again?

The purpose of creating paper prototypes is to design the user interfaces of the system-to-be so that you can run 
usability test with end-users and clients to make sure it is fit for purpose. If you discover any problem during 
usability testing, you can go back and modify your design.  By the end of the process, you have a validated 
prototype before you start coding.  Improving design on your prototype is probably going to be much less expansive 
than on your code. 

Now that you are clear on the purpose behind the task, we would like to provide some advice to help you:

### No.1: Completeness of Scenarios
During your usability test, you will have tasks for your users/clients to perform. It's really important to make 
sure that these scenarios in your paper prototype are complete. What does that mean? Let me give you an example. 

Imagine that you have a scenario where a user needs to book a hotel room.  On the interface, you have an option to 
confirm or cancel. You made sure that the "Confirm" button is clickable, and you prepared the transition to the 
next page.  But the "Cancel" button is non-clickable. During the usability test, your client clicks "Cancel" and 
nothing happens.

The example above is an **incomplete** scenario. **It's better to have 4 - 5 complete scenarios than creating 100 
pages but a lot of buttons are non-clickable**.  Remember - you want to run usability test and observe your users 
interacting with the system to improve your design. Half-completed scenarios won't help you with that - it will even 
create confusions for users/clients. If you are designing a large system and there are a LOT of user stories to 
cover, we advise you to:
1. Ask yourself: what are the most important things that users must be able to accomplish on the application? 
What user stories MUST be tested?
2. Select 4 - 5 user stories or scenarios from your list, and start prototyping. Make sure they are complete. 

### No.2: Don't Give the Answer Away
Let's use our booking hotel room example again. Make sure you don't give away clues or describe the steps to your 
users. Don't say "First you would login, then you would click the Find Destination button, then you would browse
all the hotels available, then..." the instructions that you give will prevent you from discovering design flaws. 
Instead, set up a little scenario for your users, provide them with context and observe how they complete the 
activity. For example, a better task would be:

*You are planning a trip with your family to Sydney from 24th December - 2nd January. You want to book a hotel room. 
Visit our site and see what's on offer.*

### No.3: Remember This Is a Low-Fidelity Prototype
Low-fidelity prototype shows only major navigation and content elements. You don't need to include details such as 
the colour scheme, images, styling, or meaningful content. 

### Want Some More Resources?
Check out some tutorials and resources for running usability tests in the [More Resources](#more-resources) section.

## Tips For Marvel
Here are some tips for using Marvel to create your prototype:

1. Make sure that you hide hotspot hints 
([instructions](https://help.marvelapp.com/hc/en-us/articles/360002746798-How-to-hide-hotspot-hints-when-playing-prototypes)) 
when testing your prototype with end-users/clients. Remember, one of the goals of paper prototype is to test the 
usability of your design. If you don't hide hotspot hints, end-users/clients will be given clues to know where to 
click.
2. Even with 4 - 5 scenarios, you might end up creating many of screens for your paper prototype. You can organise 
your screens into **sections** on Marvel. Checkout this series of short 
[tutorials](https://help.marvelapp.com/hc/en-us/sections/360001413858-Organising-designs-with-sections) 
on sections.

## Initial Set Up
1. Follow [this link](https://marvelapp.com/) to create an Marvel account.
2. During your sign up process, Marvel might ask you to create your first Marvel Whiteboard. You can choose "Skip for now" to ignore this option, because what you will be needing is **NOT** a whiteboard.                                                 
![](resources/Marvel1.JPG)
3. If you want to invite your team members to your workspace, keep in mind that for a free account, you can have 6 people in TOTAL (including yourself!) to **edit** the workspace projects. 
4. Using a free account, you only get ONE editable project. Keep that in mind before you create a second project.

## Create Your First Project
1. After you have signed up, you can "Create project".                                                                        
![](resources/Marvel2.JPG)
2. There will be options to choose from - select the "Prototype" option.                                                      
![](resources/Marvel3.JPG)
3. Then, enter the project name.
4. Do you know if your client wants a web-application, or a mobile app? If it is a web-application, will the users mostly access this web-app via their phone, or laptop/computer? Select a device accordingly. In this tutorial, we will go with iPhone 12. ![](resources/Marvel4.JPG)
5. Create project.

## Prototyping
- Once you have created your project, you can start prototyping! There are two stages to create your paper prototype:
  1. Design your screens - what are they going to look like?   
  2. Design the interactions and transitions between your screens. 

- Marvel offers three main ways to design your screens:
  1. Create your own design on Marvel.
  2. If you have got some design already, you can upload your design in Marvel.
  3. Use the template that Marvel provides. 
![](resources/Marvel5.JPG)

## Prototyping - An Example
Let's walk through an example.  Let's say you are designing an application for universities that will help university 
students decide which subjects to take in the future. Your clients have told you that they want the application to 
be a mobile app.

```{admonition} Reminder
Your paper prototype is an early draft of your design - it should be rapidly designed, simulated and tested with 
users. Please be careful with the level of details you put into it.  It needs to show major navigation and major 
content elements. It does **NOT** need to show colours, images or meaningful contents.
```

1. Create your first project according to the [create your first project](#create-your-first-project) section.
2. Let's design the first page - Home page. 
   - Click on "Start designing" ![](resources/Marvel6.JPG)
   - Firstly, our Home page can show some basic information about the user who has logged in. Let's create a profile 
   image icon. Select the icon options on the toolbar.                                                                             
   ![](resources/Marvel7.JPG) 
   - Let's pick the 2nd one, and add it to our design.                                                                        
   ![](resources/Marvel8.JPG)
   - Secondly, we can add some basic information about the user. Select the text option, and add text in our design.  
   ![](resources/Marvel9.JPG)
   - For now, our page looks like:                                                                                            
   ![](resources/Marvel10.JPG)
   - Next, we decide that some subjects should be listed.  They should be categorised into "Compulsory" (student 
   must complete this subject as part of the course) and "Optional". We can add some rectangles to represent subjects:                      
   ![](resources/Marvel11.JPG)
   - Our page looks like this now:                                                                                            
   ![](resources/Marvel12.JPG)
   - We are done with the design.  Let's close this page.                                                                  
   ![](resources/Marvel13.JPG)
3. Let's design the next page - a subject's page.
   - Let's create a new image.                                                                                                
   ![](resources/Marvel14.JPG)
   - According to our clients' requirements, a subject's page should have the subject's name, a description, area of 
   interests it relates to, advice from teaching staffs and past students, and a button to go back to the home page. 
   The outcome might look like:                                                                                       
   ![](resources/Marvel15.JPG)

4. Let's say we are done with our design our pages (for now).  Let's design the interactions between the two pages 
we created.
   - Hover your mouse over the Home page, click "Prototype" to add interactions. 
   ![](resources/Marvel16.png)
   - Click and drag to draw a hotspot (hotspot is an interactive area to enable users move between screens) 
   ![](resources/Marvel17.png)
   - Next, select the next screen you want to transition to. ![](resources/Marvel18.JPG)
   - Next, select the transition type. ![](resources/Marvel19.JPG)
   - Next, select the action that triggers the transition (i.e. is it a click, tap, or?) ![](resources/Marvel20.JPG)

5. Let's say we are done with designing the interactions between screens. Select the "Play" button in the top right 
corner to watch the transition you just created.
![](resources/Marvel21.JPG)
6. To share paper prototype with your client so that you can run usability test with them, click "Share", copy the 
link, and send it with them. ![](resources/Marvel22.JPG)

We hope that this simple example has helped you getting started with Marvel.

```{admonition} Extra Resources
For Usability Test
- This [tutorial](https://www.nngroup.com/articles/task-scenarios-usability-testing/) gives you more guidance and 
advice on how you should run your usability tests.
- This [article](https://www.nngroup.com/articles/why-you-only-need-to-test-with-5-users/) explains the number of 
users to run usability tests with.

For Marvel
- Marvel has a good [tutorial](https://help.marvelapp.com/hc/en-us/articles/360002536038) to help you get started 
with designing your screens and the interactions between screens - make sure to check it out!
- To find more resources for prototyping on Marvel, visits 
[this link](https://help.marvelapp.com/hc/en-us/categories/360000779958-Prototyping).
```