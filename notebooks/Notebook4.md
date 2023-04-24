# Design notebook entry

## Last week's critique

**TODO:** Fill in this part with a summary and reflection on the critique you received for
last week's work. Answer questions such as:  How, specifically, did the feedback help
improve the project? Did the feedback point out or offer something you hadn't considered?
Did it help you make a design decision? Was it helpful in addressing the most pressing
issues in your project? How will you incorporate the feedback into your work? Will you
change something about the design, implementation, or evaluation as a result?

This week I made a lot of progress because I finally figured out how to compile my code using sbt in GitHub codespaces. Last week's feeback was really helpful. I got some great advice about the data structures to use for logging foods and meals. I actually ended up using a map to store my food and meal data which was reccomended to be in class. Prof Ben was also really helpful with setting up sbt. 

## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.

This week I wanted to get to creating graphs, but I ran out of time. However I am still pretty happy with the progress that I made. The main thing I worked on was seting up my data structures. Last week, I planned on just using csv files to store all my data, but that ended up being really inconvenient. Here are the data structures I decided to use.

Weight - List[Tuple2[Int,DateTime]] 

The integer is the actual body weight and DateTime stores the date and time of the weight.

Logged Foods - Map[String, Food]

The logged foods are the foods that are saved, so that if a user wants to log the food again, they just have to provide the name, not the other details about the food. A map is ideal for this because if somone wants to change the food or add a tag, the map will replace this automatically which saves a few lines of code. 

Foods Eaten - List[Tuple2[Food,DateTime]]

This just keeps track of the time and date that each food is eaten. 

Meals - Map[String,List[Food]]]

This is similar to the logged foods, but it stores a list of foods rather than just one. 

Thinking about it now, it might be simpler to just add a list of the times the foods was eaten in the food class. This is something that I will consider next week when implementing the graph generation. I set up the food and meal functions so that you can enter them as a new or existing food or meal. If someone enters just a name, that food will be logged if it has already been created. If not, it will prompt the user about the amount of calories and tags they hope to add. 




## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

The final step of my language is setting up the graph generation which I'm hoping will be farily simple. Now that I have new data structures, I can change my calories function so that the input is a string representing the food or meal rather than the for or meal itself. Another thing that would be helpful is that if someone ate multiple of a certain food, they could specify that when entering it in in a way this is simple. It would be annoying to have to type the name of the food in 10 times if you ate that much. Another thing I want to solve at some point is possibly getting rid of the quotations when using strings as parameters. If there is a way to solve this I definitely want to use it. 

**What questions do you have for your critique partners? How can they best help
you?**

I don't really have any questions this week. I am interested to hear what types of graphs and graph designs they find the most usefull and visually pleasing. 

**How much time did you spend on the project this week? If you're working in a
team, how did you share the work?**

I spent probably about 8 hours throughout the week. 

**Compared to what you wrote in your contract about what you want to get out of this
project, how did this week go?**

I am about a week behind where I wanted to be, but I am confident I will be able to catch up. 
