Day 14 of 100
------------------

Day 14 complete!

Today I feel like I got a lot more done, I kept closer track of my time and I did 3 solid hours of practice today. This is a good way to start my week off and I am very happy about it.

During todays learning I was on the topic of Authentication and Security.

So we went over a lot of different methods that are used in terms of ways of securing your data within a database. We went over md5 encrypting, we went over encrypting then decrypting using a mongoose plugin ( name is slipping my mind ), and we learned bcrypt.js a node library.

So to break it down we went over why you should never store plain text passwords in a database ( DUH ). Which we then learned some very basic encrypt / decrypting using a key, and some preventative measures for keys using .env files and including that in your .gitignore (very useful). After that hashing was introduced and we used md5 first which was explained to actually be quite easy to break which then led us into bcrypt and salting a method that the industry uses quite a lot ( there are other layers to security as well, yes but I didn't make it that far today.)

I really like learning about this topic for some reason, it brings me back to my community college days. I really enjoy this topic and I know it can get WAY more complicated but something about the security aspect has always drawn my attention. I think it has something to do with the idea of puzzles and wanting to figure them out.

Anyways we messed around with bcrypt a bit and the concept of Salting came up and is actually quite cool. You simply add a randomly generated string of numbers ( Salt ) to whatever your password is and THEN run the hash function. For further complexity you can select a number of "rounds" so it'll hash your password multiple times, each iteration adding the Salt to the end before hashing. This ends up giving you a very long hash value which is GREAT for security purposes.

The idea is by adding this randomly generated number to the end, it helps makes your password more secure for multiple reasons.
1) It simply makes your password longer which is the number 1 way of making passwords stronger, each added character makes your password take exponentially more time to crack it. To the point where it could take years to try and break.

2) It protects people who use very basic passwords by adding random characters to the end. This helps because people have tables of hash values for basic terms, common passwords, dictionary words, and some others. So without this added layer of Salt, they could just compare your hash value to this table of theirs.

There is so much more to mention of the topic of hashing and security but I don't know where to start.

Anyways after we messed with all that we were introduced to Cookies and the idea of a Session. I've learned about this a couple times in school but I never fully grasped the concept so I am looking forward to this topic tomorrow.
