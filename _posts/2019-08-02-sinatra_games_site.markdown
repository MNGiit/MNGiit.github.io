---
layout: post
title:      "Sinatra Games Site Project"
date:       2019-08-02 22:55:45 -0400
permalink:  sinatra_games_site
---

For this project I decided on making a site that allows users to review games they have played, using Sinatra.

There are three major models: Users, Games, and Reviews. Users have attributes like name, email, and password. Games have attributes like title, and publisher. Reviews have attributes like score, and content (the wordy part of a review). A Review belongs to a User, and a Game. A Game can have many Reviews, and a User can have type (have) many Reviews.

Review is the only one that can be created, read, updated, and destroyed. The other two can mainly be created and read. Right now there isn't a way to add new games, and the games already exist in the database came from a seeds file. Eventually the responsibility for adding new games might fall on a new type of Users, the Admins of the website. Another type of Users that might exist is the Publisher. A Publisher can edit their games description. Or maybe Users can edit games too, although I think that might be a little too chaotic.

Users log in using their email, and of course password. This app uses a gem to secure User's password from prying eyes, including binding.pry. Unlike some other websites we hear on the news, I can safely say there's some work done to protect Users and their passwords.

It was interesting to see the site slowly come to life, and it felt good. Especially going back to previous lessons, or checking stackoverflow or w3schools, and trying something different.
