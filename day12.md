Day 12 of 100
------------------

Day 12 complete!

Yes today I started a bit late but hey.........the day doesn't end till I go to sleep right......

Anyways I got an hour down and I am proud of myself none the less.

Today I continued working on build my own RESTful API to help reinforce what understanding. Today I got through implementing about half the total functions.

One really cool app the course suggested using is called Postman, its quite cool actually. While developing an API it allows you to not need to code up a front end for things like testing a POST request ( where you would normally need a form or something of the sort ).

As well as learning about RESTful this time around we learned how to actually chain routes together using express. So instead of having app.get("/articles"), app.post("/articles"), app.delete("/articles") you can actually chain them together so you have one concise place to look for each route. ie..

app.route("articles")
.get( function(req, res) {
  "Whatever you want to do on .get calls to /articles"
  })
.post( function (req, res) {
  "Whatever you want to do on .post calls to /articles"
  })
.delete(function (req, res) {
  "Whatever you want to do on .delete calls to /articles"
  });

Small details but it really makes the code so much cleaner and I really like how you then have one place to look for each route.

Another thing I was practicing today which actually came up in an interview I had on Friday and it was about documenting. I was asked in my interview how well I document my code and in the spirit of honesty I admitted that I am not good at it because I haven't had any major projects that weren't for my eyes only ( This was quite embarrassing gave myself 5 / 10 ). So from now on I want to make a habit of this even though it is only for me. My thought is that it is essentially a way of taking notes and reaffirming my knowledge. And helps give me more context if ever referring back ( DUH thats what documentation is for! )
