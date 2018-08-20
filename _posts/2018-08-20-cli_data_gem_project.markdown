---
layout: post
title:      "CLI Data Gem Project"
date:       2018-08-20 19:38:18 +0000
permalink:  cli_data_gem_project
---


Recently I finished a project, and the feeling I got from it was great. This first project wanted a command line interface "to an external data source". I decided to create something that can scrape featured articles off of howstuffworks.com. It was pretty hard in the beginning, as I didn't know where to even start. The hardest part was just getting the first couple of lines of code down.

As I typed more and more code, the project got easier and easier. Of course I still had to refer back to different lessons, labs like "Student Scraper", and did some online searches. The second hardest part was using Nokogiri on howstuffworks.com. But again I just looked at previous labs, and kept trying different searches. Also, fortunately, the website's code wasn't tough, now that I think about it.

On my quest to complete this project, I had to summon some interesting methods. The .uniq method helped me get rid of repeating information in an array. So it turns out when I was collecting all the links to the articles, I would get duplicates. But thanks to .uniq, I was able to make the array just the way I needed it to be.

The pry gem is a pretty important gem I had to use. More importantly, I learned to not have binding.pry in multiple files. When one file used another, and both had binding.pry...let's just say it wasn't nice.

Another lesson I had to learn was saving my work. Many tears were shed when I would come back and see something was missing. Sometimes a lot of lines missing. I was even warned to save in the project's instructions.

Overall it was a great experience. I felt one step closer to becoming a developer.
