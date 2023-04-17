# Design notebook entry

## Last week's critique

**TODO:** Fill in this part with a summary and reflection on the critique you received for
last week's work. Answer questions such as:  How, specifically, did the feedback help
improve the project? Did the feedback point out or offer something you hadn't considered?
Did it help you make a design decision? Was it helpful in addressing the most pressing
issues in your project? How will you incorporate the feedback into your work? Will you
change something about the design, implementation, or evaluation as a result?

Last week, I didn't have much code to show so I didn't get much feedback on that, but I did get some helpful feedback on my design. I was originally planning on making a log function for logging the foods, but my feedback gave me the idea to just implicity log the food when it is created as a variable. This would save a lot of time for the end users. I have already began implementing this in my code this week. 

## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.

My main goal for this week was to get sbt working on Codespaces. However, I got sick and couldn't make it to class or any of the tutoring hours this week and still couldn't figue out how to set it up on my own. Thankfully, I figured out a way to code through a work sheet which automatically displays the output for each line without having to compile. Next week it will still be important to get sbt working. 

The code I wrote handles how to input different foods, meals, and weights. These are currently stored in csv files so that your data can be saved over time. I created four different csv files: food, meal, weight, and foods eaten. "food.csv" comtains the name of each food, the amount of calories, and any tags that are added to it. "meal.csv" contains the name of each meal and which food it contains. "weight.csv" contains the weight of each weigh-in and the date and time it occured. "foods_eaten.csv" contains the name of each food and the date and time it was eaten. 

One thing I am considering is finding a way to just save variables over time instead of using a csv file. I am not sure if there is a way to store variable on disk, but I will ask in class because that would be way more convenient than using csv files. 

Right now, a new food is automatically saved when an instance of the class Food is created.

## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

**What questions do you have for your critique partners? How can they best help
you?**

**How much time did you spend on the project this week? If you're working in a
team, how did you share the work?**

**Compared to what you wrote in your contract about what you want to get out of this
project, how did this week go?**
