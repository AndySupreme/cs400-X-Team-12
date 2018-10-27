# X-Team 12 Course Enrollment

See https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code for tips on using *Markdown* tags to format __.md__ files

## Goal

Work as a team to create a project proposal for your X-team to complete together.
The project does not have to be extremely difficult,
but there must be work to do for each member of your team.
You may reference figures using "See figure 1".  
Be sure to submit corresponding image files, i.e. figure1.png (or figure1.jpg) for each figure.

## Grading: To earn full credit, your team's proposal must include:

* (md) documentation: [this file] describing purpose and use of your program

* Description of a program that has:

  ** a main Java program class in a file named Main.java
  
  ** a custom data structure designed and built by your team
  
  ** comprehensive testing of individual units
  
 Caution: You are not being asked to implement this program, at least not yet. 
 We just want your group to make a proposal or pitch for your program.
 
 Tip: Your custom data structure can be composed of or extensions of data structures that you have learned and used in previous programming assignments.  We're looking for decisions about how to build a high-level data structure that will likely have lower-level components.

## Problem Description

Enrolling in classes can be stressful and even more so when you are placed on the waitlist. We want to improve this process by providing insight to the students on the waitlist about their current standing and how many people are in front of them. 

Our Main Class will create a priority queue that will use a text file input of the current list of students enrolls in the several classes we have in the program. Once the priority queue is created, students will be able to input their data and see if they are enrolled or waitlist. If they are waitlisted, they will be told how many students are in front of them. That calculation is based on their class ranking, pre-requisites, and major. 

We will be using a priority queue that uses a Linked List data structure. The priority queue will have several common methods that are in most queues. There will be an enqueue, dequeue, an isEmpty. It will also have a simple weighting algorithm within enqueue that will rank the priority of each student. If a student is both a senior and within that major, they are given a rank of 2. If a student is a senior/junior, or is within that major, they are given a ranking of 1. If a student only has met the pre-requisites, they are given a ranking of 0. Lastly, if a student does not meet the pre-requisites, then they are not put in the waitlist.

Testing for the priority queue will entail several types of tests for each method in the class. We will test isEmpty for it's basic functionality. We will test enqueue for its ranking algorithm and put several students in the queue with different characterstics (different ages, majors, whether or not they have the pre-requisites. Dequeue will test for both students being put into the class and for those that drop out of the waitlist. 

## Questions to answer for Exercise #2

1. Name: Give your project proposal a name (and edit the top line of this file)

Course Enrollment 

2. Output: Describe the output your program will produce.  Include and example format of the output produced.

The student's status.
Case 1: "You were successfully enrolled in class x"
Case 2: "You were placed on waitlist, there are ___ students ahead of you."
Case 3: "Waitlist full, You were not enrolled." 
Case 4: "Pre-requisites are not met, you can't enroll in this course."

3. Input: Describe the data that is needed to solve your problem. Include an example format of the input data.

Class Number, Class Maximum Size, Student Name, Student Credit Standing, Student Major, Student pre-requisites.
Example: 
Class Number: 300, Class Maximum Size: 150, Student Name: Susan Green, Student Credit Standing: 72, Student Major: Computer Science, Student pre-requisites: yes/no for CS 200.

4. User Interface: Describe a user interface for your program.  Use text menus or a simple graphic user interface.

The program front end will ask the user to put their name, student credit standing (freshman, sophomore, etc), major, pre-requisites, and class they'd like to enroll in. Example of how it would look down below:

First Name: _____
Last Name: _____
Enter Class: **drop down option**


5. Types List: Break your solution idea down into units that you think can be implemented with a single class.

We will use a class for the students in order to know basic information about them to see where they'll be place. We will also use a priority queue to implement the waitlist.

Name each interface or class and briefly describe its function or purpose.

WaitListGUI - This represents the GUI that lets the students know how close they are in enrolling in the class

StudentInfo - This class will be used for the students so that they can enter information about themselves so that it can be determined where they'll be placed in the queue

WaitList - This class represents the actual wait list of students trying to get into the class. We will implement a priority queue to handle which students will be able to enroll first


## Edit and Submit this file and any figures referenced by this document.

