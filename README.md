# DBRS_interviewChallenge

Link to Application:

https://colab.research.google.com/drive/1nQr2hnNY_9iAoU9aP6wdex1owbIbmXbv#scrollTo=_BQ62CizlZfF

1. Click on the Link
2. Colab should open, click Runtime -> Run All
3. Allow 30 seconds for all downloads and scripts to run -> Project should be running

Architecture
1. Google Colaboratory running Jupyter Notebook -> Host the application
2. Numpy and Pandas -> Python Analytics libraries
3. Matplotlib -> Display a couple graphs (It was not required, but I used it for aesthetic purposes)

Design and Tradeoffs

Originally, when planning this project, I was intending to use Docker-Compose to setup the application as noted in the original project write-up.  However, I found an even easier solution on the way to get everything up and running - Google Colaboratory.  

Docker is great - there is no doubt about that.  However, for this project, quick onboarding was highly emphasized in the project instructions so that the code can be setup and reviwed with the most minimal of instructions. With 1 executing python, script, there was not much infrasture as code, (databases, ports etc..) - what docker shines in.  

Furthermore, anyone, anywhere around the world, even with basic computer knowledge, can access the application and run the whole project with only mouse clicks - no need to even type or use the keyboard!  To get the project up and running with docker, you would need to have an operating system built on a linux kernal (windows users can't do anything), Docker downloaded & installed, images downloaded, and execute docker command scripts - even a command to turn docker off after reveiw. With Colaboratory, just click the X on the browser. Docker is great for a microservice-type architecture, one built with databases and possibly differnt programming languages, of which you could update a part of an application without having to update the other part.  

With efficieny in mind, this application is too light-weight for such purposes, although it is possbile to use Docker.  Additionally, the project seems to be very data-science heavy, and probably suitable to be read by a data scientist, who may not be as savvy with setting up docker, running, or even be able to understand it within a short time.  

Project Instructions:

All tasks below completed. 

-Consider only the 10 most common overall complaint types. For each borough, how many of each of those 10 types were there in 2017?

-Consider only the 10 most common overall complaint types.  For the 10 most populous zip codes, how many of each of those 10 types were there in 2017?

-Considering all complaint types. Which boroughs are the biggest "complainers" relative to the size of the population in 2017? Meaning, calculate a complaint-index that adjusts for population of the borough.

