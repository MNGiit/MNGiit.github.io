---
layout: post
title:      "Rails Recipe Manager Project"
date:       2019-10-02 21:22:12 +0000
permalink:  rails_recipe_manager_project
---


For my third portfolio project, I decided to make a recipe manager, using Rails.

First the person has to be able to sign up. Similar to my Sinatra project, user signs up with a name, email, and password. Also like the previous project, the Bcrypt gem is used for password security. But suppose a user doesn't want to sign up like that...well they're in luck. It's possible thanks to Omniauth, and Omniauth-github gems. But the user would need to have a github account if they want to log in from this method.

Once the user logs in they can begin making their own recipes. A user can create, view, edit, or delete their review. User can see other recipes by other users as well. Recipes belongs to user, and it can have many ingredients. Recipes can also have many reviews, and through reviews, many ratings.

A user can leave a review on another user's recipe. The review is basically a user rating. Reviews belong to users, and recipes. And the rating belongs to the review.
