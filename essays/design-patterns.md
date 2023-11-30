---
layout: essay
type: essay
title: "Are Design Patterns setting you up for success or failure?"
# All dates must be YYYY-MM-DD format!
date: 2023-11-29
published: true
labels:
- Design Patterns
- Software Engineering
- Reflection
---
## Introducing Design Patterns...
If you are an owner of a bakery that is known for its delicious desserts, consistency in taste and providing exceptional service to customers are crucial goals. In order to make your bakery the best in town, you have designed different solutions in order to address recurring problems that you see in your business operations. Although software engineers typically don’t bake cakes, they similarly develop solutions to recurring problems within their code, known as Design Patterns. Failing to implement design patterns in your software engineering projects can resemble baking one batch of cookies overly sweet and another batch far too bland. Such inconsistency lacks organizational structure and coherence. You want to have a recipe for your pastries, something that is understandable and clear for your workers to bake the desserts perfectly. In the future, you can reuse recipes for a vanilla cake to make a chocolate cake. You want your code to be designed and implemented in the same way.

## Meteor's implementation of Design Patterns
While working on the Hawaii Annual Code Challenge (HACC) along with my 2 group members, the concept of design patterns were unclear. We wanted our application to have different features and functionalities as soon as possible, however, creating code that followed these design patterns was difficult. Since we used Meteor to create our project, it simplified our solutions for complex problems and implemented some concepts of these design patterns. One of our project features is the report system. User’s can report any chatbot messages that they believe are inappropriate, incorrect, or lack useful information. To hold all of this data, we saved it into a MongoDB collection. Whenever a report is submitted, the MongoDB is updated and anything subscribed to the collection reruns. In this case, the reports page was subscribed to ‘reports’ MongoDB collection and the code is rerun in order to display all of the new reports. Meteor’s “reactivity” is an example of the Observer design pattern.


## Should everyone use Design Patterns?
Several design patterns can often be complex and difficult to understand, leading some software engineers to misuse them to inappropriate problems. This misuse can make your code more complicated rather than solving the actual problem. Admittedly, both my teammates and I are guilty of not following some design patterns, however, we didn’t want to write code in a way where we couldn’t understand what we were doing. I think some software engineers attempt to implement design patterns without a complete grasp of their concepts, sometimes driven by time constraints or lack of motivation. I've personally found myself in situations where I just need to get my code working, only to realize that this way of coding is more detrimental to my software engineering learning than any good. Although me and my teammates did not implement some design patterns into our project, we built our project with the purpose of learning more about software engineering. If you are a complete beginner to software engineering, I think it is totally fine to not implement some design patterns in your code right away. Get down the basics first, then you can slowly learn about all of the other design patterns. With years of experience and practice, you can make design patterns seem as simple as pie!

