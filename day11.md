Day 11 of 100
------------------

Day 11 Complete!!!

Had a really good day today.

Had my first interview for a tech job ( in almost a year ) and I am so glad I got interviews coming in now. One of the more exciting parts of the interview is where they allowed me to show some of the things I have been working on. So I showed them the todo list project that is hosted on MongoDB Atlas / Heroku which was exciting and I also showed them the website I am creating for my very first real client.

Today in my learning I converted the old Blog website that we made using static arrays into one that uses mongoDB. It was a challenge so we weren't just following along. We were prompted on what was needed / wanted and we had to do it. This method really reinforces what we are learning and I enjoy it. Show us once let us follow along and then have us do it on our own. And surprisingly I only had to look back at the docs for one or two things ( one of which we had never done before.)

There was an interesting error that occurred which I hadn't even been thinking of as a possibility.

After we .save() our new document, in this case our new blog post. It should save the document to the database and then redirect us to another page. On this page that we are redirected to it shows the Title and a preview of the post ( 100 chars ).

Well after you run .save() depending on the size of the post's content it might take longer than the immediate call to redirect. In this case you will be redirected but the new post might not have finished being written and so it won't display till you refresh.

So what we did is put the redirect into our .save() call's callback function.

Post.save(function(err) {
  (!err) {
    res.redirect("/");
  }
  });

Obviously this example is not very complicated but it is quite cool. You can do all sorts of things with knowing this.

Other than that I started learning what it means for an API to be RESTful, I learned which Verbs we are allowed to use: GET, POST, PUT, PATCH, and DELETE. Which is essentially C.R.U.D GET = Read, POST = Create, PUT / PATCH = Update, and DELETE = Delete. I love when things start to connect! :)
Aside from the verbs we are allowed to use, we went over the standards of what/how your endpoints/routes should be and are to be used. This is so nice that these standards are set in my opinion. It makes the world of coding just that much less of a free for all.

That was just about it for today, I got through the set up for our next project where we actually are creating a RESTful API, that will be tomorrows adventure.
