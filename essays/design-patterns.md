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
<img src="../img/design-patterns/design-patterns.png" width="600px">

## Introducing Design Patterns...
If you are an owner of a bakery that is known for its delicious desserts, consistency in taste and providing exceptional service to customers are crucial goals. In order to make your bakery the best in town, you have designed different solutions in order to address recurring problems that you see in your business operations. Although software engineers typically don’t bake cakes, they similarly develop solutions to recurring problems within their code, known as Design Patterns. Failing to implement design patterns in your software engineering projects can resemble baking one batch of cookies overly sweet and another batch far too bland. Such inconsistency lacks organizational structure and coherence. You want to have a recipe for your pastries that is understandable and clear for your workers to bake the desserts perfectly. In the future, you can reuse recipes for a vanilla cake to make a chocolate cake with some alterations. In software engineering, you will be working with other groups of people, so making understandable and reusable code is crucial just like how it is for baking pastries.

## Meteor's implementation of Design Patterns
While working on the Hawaii Annual Code Challenge (HACC) along with my 2 group members, the concept of design patterns were unclear. Our primary goal was to quickly incorporate diverse features and functionalities into our application. However, creating code that followed these design patterns led to many challenges. Since we used Meteor as our development platform, it simplified our solutions for complex problems and allowed us to implement certain aspects of these design patterns.

One noteworthy feature in our project is the report system, which allowed users to flag chatbot messages that they believe are inappropriate, incorrect, or lack useful information. To manage this data, we saved it within a MongoDB collection. When a report is submitted, the MongoDB is updated , triggering a rerun of anything subscribed to the collection. In this case, the reports page was subscribed to the ‘reports’ MongoDB collection and the code is rerun in order to display the updated reports.

Meteor’s “reactivity” is an example of the Observer design pattern, where changes in data trigger automatic updates to the subscribers in the application. By implementing this design pattern, we were able to reuse this code easily for our FAQ page, with some minor alterations. This saved us some time while also using a small amount of code:

```
const ReportsPage = () => {
  // Reactive data for the reports database
  const reports = useTracker(() => ReportCollection.find({}).fetch());

```

## Should everyone use Design Patterns?
Several design patterns can often be complex and difficult to understand, leading some software engineers to misuse them to inappropriate problems. This misuse can make your code more complicated rather than solving the actual problem. Although me and my teammates did not use all of the different design patterns, we didn’t want to write code in a way where we couldn’t understand what we were doing. I think some software engineers attempt to implement design patterns without a complete grasp of their concepts, sometimes driven by time constraints or lack of motivation. I've personally found myself in situations where I just need to get my code working, only to realize that this way of coding is more detrimental to my software engineering learning than any good. Although me and my teammates did not implement all of the different design patterns into our project, we built our project with the purpose of learning more about software engineering. If you are a complete beginner to software engineering, I think it is totally fine to not implement some design patterns in your code right away. Get down the basics first, then you can slowly learn about all of the different types of design patterns. With years of experience and practice, you can make design patterns seem as simple as pie!


