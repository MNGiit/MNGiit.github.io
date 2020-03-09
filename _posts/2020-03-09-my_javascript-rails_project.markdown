---
layout: post
title:      "My JavaScript-Rails Project"
date:       2020-03-09 05:06:38 +0000
permalink:  my_javascript-rails_project
---


For my JavaScript Rails project, I decided to make an app that can give visitors a short quiz or exam on things related to Web Development. Of course I would have to understand it or else the questions will be bad. So it also gives me a decent excuse to go over the material myself.

Before I begin making it, I will first have to consider what will go in. At the minimum it will be a short quiz. And a quiz has questions. It looks like I can use two models, one for quiz, and one for question. If a user wants to take a quiz on HTML, then the questions should all be related to HTML. Another model I can use can be topic.

The relationships or associations can be something like:
quiz has many topics
quiz has many questions through topics
question belongs to quiz
question belongs to topic
topic has many quizzes
topic has many questions through quizzes
I might change how it is as I make the app.

There are different kinds of questions, so for now I'll stick with multiple choice questions. A question would have at least four choices for the user to select. And only one correct answer.

The next thing to consider is when to check for correct answers and calculate the score. I could have it done on the user's browser. Or I can have it sent to the server when the user is done taking the quiz, and let the server figure it out. I might make it so the server calculates the score, but as I make it I might change my mind.

When the user is done, and gets their score, what should happen next? I might add a high score leaderboard for each kind of topic. So the user will see the leaderboard and if they make it in they can leave their score and name. This might make it more like a video game so I'm not sure about it. In any case the user will be asked if they want to retake it or take another kind of exam.
