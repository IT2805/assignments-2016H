# Assignment 7: JavaScript continued

Are you having trouble remembering what you have to do? Great news everyone! In this assignment you will make a todo list.

Your submission shall consist of two files, an HTML page named `todo.html` and a JavaScript file named `todo.js`. Go ahead and create them, and we will get along with this exciting exercise.

Deliver the two files in a zip file on itslearning.

## Part 1: Prepare the HTML file (10%)
The HTML page should consist of a title, one button for adding tasks, a correlating input field, an output element, and a list where the tasks are presented. Make sure to add IDs on the appropriate places.

When the user enters the page, the input file shall automatically get the focus.

Connect your HTML page with the JavaScript file. The rest of the task should be done in the JavaScript file.

## Part 2: Implementing Functionalities (20%)
Now we (read: you) will start to implement some functionality.

When the user writes a task in the input field and clicks the add button, the task shall be added to the empty list with a checkbox in front of it. Make a JavaScript functions named "addTask()" that does this.

Hint: Use eventlisteners to listen on button clicks.  
Hinter: If you want to remove the list bullet, you can do so using CSS.  
Hintest: Use `preventDefault()` so that the page does not reload itself if you use a form.  

## Part 3: Storing Users' Activities (20%)
Instead of just showing the tasks in the DOM, we also want to store them as an object, so that we can make changes to a task.

In `todo.js` you should create an empty list called `tasks`. Then expand your function "addTask()" so that it adds a task object to the list. The object should consist of the attributes:
* timestamp
* task

The timestamp could be the number of milliseconds between 1 January 1970 00:00:00 UTC and now (i.e. use the JavaScript Date object). The task should be a string.

## Part 4: Adding more Functionalities (25%)
If the user checks the checkbox, the following should happen:
* the task should have a line through it
* the task should be moved below the tasks that are not completed

Should the user uncheck the checkbox, the task should be reverted to it's default state (no line through and sorted with the uncompleted tasks).

Hint: Use the timestamp as an ID for the task.  

## Part 5: Making it Interactive (25%)
We have not forgotten about the output element. Every time you update a task (check it, uncheck it or add it) the output element should be updated with the number of completed tasks and the number of tasks. E.g. if you have 7 tasks and 3 are completed, it should read '3/7 completed'.

## The encouraged last part
Style your todo list to look smashing using CSS. This part will not be graded, but is a nice task when you do not want to do your assignments in other courses.

## Deliverables
Submission should be uploaded as a zip file into It’s Learning before the deadline. Submissions are ONLY accepted via Its Learning. We DON’T accept late assignments. Emails or any other messages with late assignments are automatically discarded without further communication
