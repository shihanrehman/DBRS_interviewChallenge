# DBRS_interviewChallenge

Link to Application:

https://colab.research.google.com/drive/1nQr2hnNY_9iAoU9aP6wdex1owbIbmXbv#scrollTo=_BQ62CizlZfF

1. Click on the Link
2. Colab should open, click Runtime -> Run All
3. Allow 30 seconds for all downloads and scripts to run -> Project should be running

Architecture
1. Google Colaboratory running Jupyter Notebook -> Host the application
2. Numpy and Pandas -> Python Analytics libraries
3. Matplotlib -> Display a couple graphs (It was not required, but I decided to use it for aesthetic purposes)

Design and Tradeoffs

I decided to use Google Colaboratory instead of Docker-Compose as suggested in the challenge.  

Docker is great, but for this project, I was very limited to what I could do with docker and 'infrastructure as code'- what docker shines in - no databases, no ports, etc.. ) - only a single python file.  Getting the application up and running quickly was also highly prioritized - so I wanted to keep execution as simple as possible.  Quote - "Please consider the fact that we have to get onboarded with your project so adding good documentation for us to follow to set it up is nice to have."

Aditionally, anyone from anywhere around the world with an internet connection - even with no programing knowledge, can get the application up and running in less than a minute with just a couple mouse clicks - no need to even type or use the keyboard!  

To get the project up and running with docker, one would have to have an OS built on top of a linux kernal - even with a linux system, Docker has to be downloaded & installed, images have to be downloaded, and commands need to be executed via command line to run the containers - even to shut down the containers!   Docker is great for microservices and deploying them - perhaps, an application built with differnt databases and programming languages all running independently of one another on connected ports via a docker-compose yaml file, making it with possibile to update one part without having to the update the other.   

With efficieny in mind, and this project being very data-science focused, I am also guessing that a data scienctist - someone who may not be familiar wtih docker and infrastructure code, may want to have a look at it.  

Google Colaboratory also has an option where you can create tabbed menus, similar to a tabbed jorurnal/phonebook, making it easy to separate the code into sections by topic. This makes visual presentation and reporting much more appealing.     

I tried to keep my code as minimal and short as possible.  However, I did write some extra code - only to generate graphs and do some validation, but nothing more than what was needed for other than those purposes.    

Everything is setup is one Jupyter Notebook running on the cloud.    

Project Instructions:

All tasks below completed. 

-Consider only the 10 most common overall complaint types. For each borough, how many of each of those 10 types were there in 2017?

-Consider only the 10 most common overall complaint types.  For the 10 most populous zip codes, how many of each of those 10 types were there in 2017?

-Considering all complaint types. Which boroughs are the biggest "complainers" relative to the size of the population in 2017? Meaning, calculate a complaint-index that adjusts for population of the borough.

