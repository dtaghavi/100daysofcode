Day 7 of 100
------------------


Day 7 completed!!

Today started off kind of annoying. As I mentioned in a previous day, I hate getting things set up in a new environment / fresh computer or whatever it may be.
I always feel on edge about file paths etc.. something can go wrong so easily I feel like. Hopefully the more experience I gain this feeling will go away.
So today before getting started I updated my MacOS to Catalina.

Uh-Oh!
Something broke.........  

I go to start my lesson for the day where I am continuing with MongoDB using Mongoose aaaaaaand I can't start up my MongoDB server.

As you can imagine I copy the errors and go to google and pray to the Stack Overflow gods that they have a solution. I tried a couple different things and couldn't get it to work.
Finally I found a post someone had made on how to get it all working ( about 30 min later ) and whoever this angel was make a clear and easy to follow post about it.

I will link it here incase anyone else has this issue.
https://zellwk.com/blog/install-mongodb/

But basically the issue was ( aside from having to reinstall using Homebrew ) typically you would place your database files in the root directory "/". Well apparently in Catalina writing to files in the root directory is a no no. Which was the recommended default of mongodb, or at least what everyone did. Anyways other than that the commands to run / check status / turn off the server changed as well. But that handy little link I put above he shows you how to create some nice little alias' for each command. I never knew you could do this but the idea is pretty straight forward you assign the command to a variable essentially ( alias ). God I love learning more about programming.

Anyways after this fiasco I got to work on my course, although I suppose the above was a learning situation too LOL. I got through the basic CRUD functions using mongoose with node. I gotta say anyone who has to use the native driver of node to use Mongo must have the patience of a god. Because Mongoose really simplifies things SO much, its great.

I am going to commit my project with all those basic CRUD functions to this Git Hub if anyone wants to see.

Make sure to follow me on Twitter as well @DTaghavi ! Thanks for reading and message me on Twitter if you'd like to share anything.
