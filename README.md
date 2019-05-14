# 401 Advanced Javascript

## Course Goals

### Students will be able to demonstrate ...
* Complete mastery of JS Fundamentals
  * Objects, Factories, Classes
  * Standard and Arrow Functions
  * Looping, Iteration, Traversal of Arrays and Objects
  * Recursion
  * Documentation best practices with JSDoc
* Understanding of core data structures
  * When each structure is most appropriate
  * Real world applicataions of each structure
  * Looping, Iteration, Traversal
    * Stacks & Queues
    * Linked Lists
    * Trees
    * Graphs
    * Hash Tables
* Creation and operation of an Express web server
  * Static Routes
  * Dynamic Routes
  * EJS
* Creation and operation of an Express API Server
  * RESTful, Dynamic Model Management
  * Authenticated Access with RBAC
  * Swagger Documentation
* Creation and operation of a Socket.io Message Queue Server and Client Library
* Creation of a single page web app in React
* Creation of a mobile app with React Native
* Deploy a website to AWS, Heroku, Zeit, Netlify, GoDaddy
* Deploy an API & Lambda functions at AWS

### Course Takeaways / Alumni Toolkit

* Reliable, Scalable API Server
* Reliable, Scalable WWW Server
* Message/Queue Service and Client Library
* React/Redux Starter App
* React Native (Mobile) Starter App
* Stable of React and React Native Components at NPM (Styled)
  - `<Header />`
  - `<Footer />`
  - `<Modal />`
  - `<Auth />`
  - `<Rotator />`
  - `<Autocomplete />`
  - `<Draggable />` and `<Droppable />`
* Scalable SASS Layout and Theme Engine

## Course Layout and Operations

### Daily Lecture and Labs

The facilitators folder in each day contains information for the instructional staff. Your daily lecture schedule should follow a format similar to the following, adjusting for your class needs.

**Hour 1**

Use the first hour to start the day cleanly with announcements, code review and optional extra material. Time is alotted for optional exercises such as an on the fly quiz, demonstrating (or pair programming with a student) one of the daily/weekly warm-ups or doing a live white-board session with one student. All are valuable, and should be rotated by the instructor based on the needs and rhythm of the class.

* :05 - Introduction, Welcome, Announcements
* :15 - Lightning Talk (1 Student per day)
* :20 - Review / White Board / Warm-Up
    * Q&A (Quiz Style) review of course material
    * White Board Practice with one student, live
    * Complete one of the daily/weekly warm-ups for or with (paired) the students
* :20 - Code Review

* BREAK

**Hour 2**

During the 2nd hour, introduce a new CS or UI concept as a short warm-up. This is a great time to squeeze in some CSS tricks, review recursion or reinforce anything that the students need clarification on. Close the hour with a solid presentation of the new material and topic for the day. This is where you'll do drawings, share a powerpoint and do your more traditional "lecture"

* :30 - UI, Design, or CS Concepts 
    * i.e. SASS, Menu Styling, Design Pattern, DS&A Practice/Review
    * Use this time to fill in gaps or elevate skills
* :30 - Lecture on the new concept of the day
    * Slides, Drawings, Examples, Etc.
    * This should be mostly conceptual and high level

* BREAK

**Hour 3**

Finish the day with a live coding demo that supports the class topic and sets the students up for executing their lab.

* :55 - Live Code Demo
    * Supportive of the day's principle concept
* :05 - Lab Preview
    * Go over the LAB, DESIGN, and WARM-UP assignments and set expectations

### Guide Repo Setup

* Run the included `setup-401-js` shell script to create your guide repo
* To do this manually instead ...
  * Create a repository with your class code, and copy the following into it:
    * `README.md`
    * `demo` folder
    * `lab` folder

The `DISCUSSION`,` DESIGN`, `WARMUP`, and `LAB` assignments are linked automatically into Canvas, but are in the guide repo for your review.

* `/apps-and-libraries`
  * Storage home for the "golden" apps built in class (see above)
* `/configs`
  * Re-usable configuration files for Travis, .git, Linting, etc.
* `/curriculum`
  * `/class-##` - Daily Lecture Folder
    * `README.md` - The daily "go" file for the students. Edit this each day with any notes or announcements.
    * `DISCUSSION.md` - The daily reading assignments for students.
    * `REVIEW.md` - A set of "pop-quiz" style questions tailored for each day to keep students connected to older topics.
    * `/demo` - Contains fully baked lecture demos and notes
    * `/facilitator` - Contains lecture notes, assets, solution code
    * `/lab` - Contains all assignments
      * `/LAB.md` - The core lab for the day
  * `data-structures`
    * Contains javascript specific notes and demo code for each  structure.
    * This material is designed to **augment**, not replace the core curriculum materials
  * `/design-assignments`
    * Contains the design assignments and solution code
    * Contains the daily design assignments. 
    * These are not included in the daily folders to allow for the design assignments and the daily labs to operate independently.
    * These are automatically pulled into Canvas from this folder.
  * `/projects`
    * Contains the lab instructions, solutions and notes for the midterm and final projects
  * `/warm-ups`
    * Contains warm-up lab assignments and solution code
    * These are not included in the daily folders to allow for the design assignments and the daily labs to operate independently.
    * These are automatically pulled into Canvas from this folder.
* `/reference`
  * Contains reference information, templates, how-to's, cheat sheets, etc.    
* `/extra-content`
  * This is an open area for 401 instructors and staff to do curriculum development
  * In here, setup new course materials as a properly formatted "day" which can be taught independently.
  * These can be rolled into the course in the future or taught as supplemental or replacement lectures as required/possible

## Student Operation

#### Students will **fork** the class repository
On most days, the lab folder will have some starter-code for them to copy. They will generally be making a new repository each day and copying that code in as a starting point.

It's advisable that the students first make an new org (perhaps called '401-js-<their-name>') that these repositories can be created in, to help them organize things better.

### ASSIGNMENTS

  * **READING (Due before each lecture)**
    * Source: `DISCUSSION.md`
    * Linked directly into Canvas from the Guide Repo
    * Reading assignments should be done as articles/notes in the **wiki** of their repo fork
    
  * **DS&A CODE CHALLENGE (4 per block)**
    * 5 points (3 points for whiteboard, 1 point for testing, 1 point for working code)
    * ~ 1 Hour
    * Source: `common-curriculum/data_structures_and_algorithms/Code_401/class-[05/10/15/...]/LAB.md`
    * Linked directly into Canvas from the Guide Repo
    
  * **LAB Assignments (4 per block)**
    * 10 Points (graded on the rubric)
    * ~ 3 Hours
    * Source: `curriculum/class-[##]-[name]/lab/LAB.md`
    * Linked directly into Canvas from the Guide Repo
    * Should be completed in a new repository for each day
    * Generally, these are smaller implementations, refactors, and practice to support the lecture concept. Not necessarily a full-scale application.
    * Code must be tested through Travis and deployed through either Heroku or AWS
    * JS Code must be documented with JSDoc
    * APIs must also be documented with Swagger
    * Students must use the README.md template to complete their assignment
    * The README requires them to have links to deployed code, Travis, functional documentation, test documentation and a UML and/or data-flow diagram.

  * **DESIGN (1 per block)**
    * 10 Points (complete/incomplete)
    * 1-2 Hours
    * Source: `design-assignments/DESIGN-[01,02,03,...]
    * Linked directly into Canvas from the Guide Repo
    * Following a short lecture at the end of each block, students will iteratively build out a scalable "design" or "theme" which should be easily transferable to any project they do.
    * This will be both monolithic and componentized (depending on how they implement it: Static or React).
    
  * **DS&A IMPLEMENTATION**
    * 10 Points (complete/incomplete)
    * Source: `common-curriculum/data_structures_and_algorithms/Code_401/class-[05/10/15/...]/LAB.md`
    * Linked directly into Canvas from the Guide Repo
    * There is an associated reading with each of these "Day 5" lectures/labs
    
  * **END OF BLOCK PROJECT**
    * 25 Points (graded on the rubric)
    * 2 Days (weekend for day class)
    * Generally Paired
    * Takes the learnings/components/modules from the previous 4 classes and has the students assemble them into a larger/full-scale application.
