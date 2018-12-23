                                            # DBRS_interviewChallenge
                                            
                                            
                                           Video Demo via Youtube Screencast
                                            
                                            

                                          Instructions to Run Application


https://colab.research.google.com/drive/1nQr2hnNY_9iAoU9aP6wdex1owbIbmXbv#scrollTo=_BQ62CizlZfF

1. Click on the Link
2. Colab should open, click Runtime -> Run All
3. Allow 30 seconds for all downloads and scripts to run -> Project should be running

                         
                         Architecture and Assumptions about Design and technology tradeoffs


1. Google Colaboratory running Jupyter Notebook -> Host the application
2. Numpy and Pandas -> Python Analytics libraries
3. Matplotlib -> Display a couple graphs (It was not required, but I decided to use it for aesthetic purposes)

I decided to use Google Colaboratory instead of Docker-Compose as suggested in the challenge.  

Docker is great, but for this project, I was very limited to what I could do with docker and 'infrastructure as code'- what docker shines in - no databases, no ports, etc.. - only a single python file.  Getting the application up and running quickly was also highly prioritized - so I wanted to keep execution as simple as possible.  Quote - "Please consider the fact that we have to get onboarded with your project so adding good documentation for us to follow to set it up is nice to have."

Aditionally, anyone from anywhere around the world with an internet connection - even with no programing knowledge, can get the application up and running in less than a minute with just a couple mouse clicks - no need to even type or use the keyboard!  

To get the project up and running with docker, one would have to have an OS built on top of a linux kernal - even with a linux system, Docker has to be downloaded & installed, images have to be downloaded, and commands need to be executed via command line to run the containers - even to shut down the containers!   Docker is great for microservices and deploying them - perhaps, an application built with different databases and programming languages all running independently of one another on connected ports all defined via a docker-compose yaml file, making it with possibile to update one part without having to the update the other.   

With efficieny in mind, and this project being very data-science focused, I am also guessing that a data scienctist - someone who may not be familiar wtih docker and infrastructure code, may want to have a look at it.  

Google Colaboratory also has an option where you can create tabbed menus, similar to a tabbed jorurnal/phonebook, making it easy to separate the code into sections by topic. This makes visual presentation and reporting much more appealing.     

I tried to keep my code as minimal and short as possible.  However, I did write some extra code - only to generate graphs and do some validation, but nothing more than what was needed for other than those purposes.    

Everything is setup is one Jupyter Notebook running on the cloud.    

                                                        
                                                        Project Instructions
                                                        

All tasks below completed. 

-Consider only the 10 most common overall complaint types. For each borough, how many of each of those 10 types were there in 2017?

-Consider only the 10 most common overall complaint types.  For the 10 most populous zip codes, how many of each of those 10 types were there in 2017?

-Considering all complaint types. Which boroughs are the biggest "complainers" relative to the size of the population in 2017? Meaning, calculate a complaint-index that adjusts for population of the borough.


                                                          Data Cleansing
                                                          

I took into account funny characters found in the data, particular in the zip codes colum, as well as a few others.


                                                          Data Sources


1. I was able to source the data from here, https://dev.socrata.com/foundry/data.cityofnewyork.us/fhrw-4uyv - on the site, I was able to filter data for 2017 and export it to CSV.  The CSV file, being about 1.2 GB in sized, was downloaded, zipped to 100MB, and stored in dropbox.  The application downloads the data set and unzips it upon execution.


2. I was able to souce the population by zip code data from here: https://blog.splitwise.com/2013/09/18/the-2010-us-census-population-by-zip-code-totally-free/.  The CSV file is in the kilobytes, so it was stored into dropbox.  The application downloads is upon execution.  

