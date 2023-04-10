# Design notebook entry

## Last week's critique

**TODO:** Fill in this part with a summary and reflection on the critique you received for
last week's work. Answer questions such as:  How, specifically, did the feedback help
improve the project? Did the feedback point out or offer something you hadn't considered?
Did it help you make a design decision? Was it helpful in addressing the most pressing
issues in your project? How will you incorporate the feedback into your work? Will you
change something about the design, implementation, or evaluation as a result?

The feedback from last week was really helpful because I had to make some big decisions for my project and it was great to get another opinion on those choices. One piece of feedback that I found really helpful was the idea to add the ability to track vitamins and minerals as well. This is something important for vegetarians and not a lot of nutrition tracking apps have these features. This gave me the idea to add tags to each food item whoch will give users the ability to associate each food with any number of tags that they create themselves. This allows users to track the things that they care about for their own personalized diet. 

## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.

This week I mainly have been working on designing my language in Scastie. I have been trying to set up sbt on GitHub codespaces, but have ran into a lot of issues with that, so I have been using Scastie to test things out while I set that up. I have been playing around with the classes for different types of food entries. Each food has an assigned amount of calories that can be returned. Ideally the foods can also be grouped together into meals. For example, let's say that pizza is 200 calories and soda is 100. To log this as a meal you would enter:
food(pizza, 200)
food(soda, 100)
meal(comboMeal, pizza, soda)
log(comboMeal)
The reasoning behind making it this way is so that if that is a meal that the user repeatedly has, then in order to log it again all the would need to type is just "log(comboMeal)". If it is a meal they they think they will only have once, they could alternatively log it like this:
log(food(pizza, 200), food(soda,100))
This would be faster, but it wouldn't save as a meal. I have been struggling to set up my actual codespace. I haven't really been able to get SBT to work. I hope on Monday I could get some help from my classmates or the professor. Right now my ain problem is that it just gets stuck loading when I try to commit to GitHub. 

## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

Right now the most pressing issue is to get Codespaces to work, but that is not something I am worried about because I am sure with some help from the class I can get it working. Then I need the finish implementing the log function to enter in data. 

**What questions do you have for your critique partners? How can they best help
you?**

I was wondering if it would be helpful to be able to edit meals or food items after you create them. For example, if you entered the amount of calories for a specific food item in wrong and wanted to change it, would it be helpful to be able to edit it, or would it be more convenient to just make a new one?

**How much time did you spend on the project this week? If you're working in a
team, how did you share the work?**

I am estimating I spent about 6 hours this week on my project. About 2 hours in Scastie, 2 hours working on CodeSpaces, and about an hour journaling and doing critiques. 

**Compared to what you wrote in your contract about what you want to get out of this
project, how did this week go?**

This week was really slow due to the porblems with Codespaces. I definitely need to pick it up next week if I want to stay on track, but I am confident that once I get Codespaces working I will be able to catch up.
