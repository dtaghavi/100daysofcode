Day 13 of 100
------------------


Day 13 is complete!

Weekends can't stop me!

So today I finished up the module on creating a fully RESTful API. I did this using a Wikipedia type site example.
In it we didn't develop any front end, so a good way of using and testing it, like I mentioned yesterday, is an app called Postman(check it out.)

Anyways I did commit the project to my GitHub if you wanted to check it out and I made a point of documenting it quite a bit. Admittedly for myself to use as a reference in the future but also to practice my documentation skills. Which gets me thinking what are some standards on documentation I should really look into this ( send me some if you know of any via Twitter. @DTaghavi)

One of the cool things about RESTful is the difference between PUT and PATCH. Really the ideas of a RESTful architecture are very nice, it just makes things more consistent and helps developers know what to expect.

So for PUT you will replace ENTIRELY a currently existing document. The new document that is created will only contain the fields provided. For example, lets use our Wikipedia example, there are only two fields {tile: String, content: String}. So when make your PUT request if you only provide a new {content: "Interesting"} in the request, your current document of lets say {title: "RESTful", content: "Is amazing"} will be REPLACED with an entirely new document containing {name: "Interesting"} and you will lose your title field.

To contrast it PATCH will simply update your current document with the fields you provide. For example lets use the same scenario as above. {title: "RESTful", content: "Is amazing"} is your current document, you then make a PATCH request containing only {content: "Interesting"}. Your UPDATED document will look like this, {title: "RESTful", content: "Interesting"}.

Anyways, the idea of setting standards for how endpoints should be used is nice to see, and makes things easier to understand. I like when standards are set so everything isn't different in every code base. ( If they are followed at least. ) I wonder how often you see APIs that say they are RESTful and aren't actually.

Tomorrow I will be diving into the next module about Security.
