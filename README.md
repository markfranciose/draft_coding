# Introduction

> "First principles, Clarice. Simplicity. Read Marcus Aurelius. Of each particular thing, ask what is it in itself? What is its nature?"  **Hannibal Lecter**
   
The purpose of this introduction is to briefly name the ideas that should underly Ekta's coding standards.

## Write in the language (and community) you're writing in.
In general, use the popular conventions of the language or framework, unless there's a good reason not to. Perhaps you like Elm and dislike TypeScript. Fair enough. However, be a good citizen and write your TypeScript the way Typesceipt is typically written. Ekta's standards are designed to align with the current habits of particular communities. When a consensus doesn't exist, do what's best for the whole team -- which leads us to...

## Write code for people. Especially the people on your team. Talk to the people. 
(Most) everyone agrees that the first part of the header is important. How to exactly do that, gets dicey. There are lot of suggestions, many ```<strong />``` suggestions, in these guides and fewer rules. Ultimately, we're trying to find the best trade-off between creativity and productivity. If the team for a project wants to use Allman-style brackets in a Javascript project, and it matters enough to make people even consider the topic, fine[3]. Real communication between team members is more important than even convention. A specific way to actualize this is to spend 0 minutes in all level of code reviews talking about brackets.

Another reason to be (bendy) on this is to allow the space for people to be creative. More on this in the 'Being Cool' section. Pro comments, pro verbosity . 

# Being Cool
The purpose of this section is to allow areas for people to be cool.

Consider the following Ruby method:
```ruby
def add_columns
  a = [1, 2, 3]
  b = [4, 5, 6]
  c = [7, 8, 9]
  
  [a,b,c].transpose.map { |x| x.reduce :+ }
end
```
On one hand, without a fairly good knowledge of Ruby someone looking at your code probably doesn't understand what that code does (and then try explaining to them why). On the other hand, the implicit return statement above is sweet[4]. Being sweet feels good. Despite any subtrefuge about diskspace, (other excuses) being cool is good for its own sake. The problem is don't let your coolness mess up other people. To that end, a glorious solution presents itself:
```ruby
def add_columns
  a = [1, 2, 3]
  b = [4, 5, 6]
  c = [7, 8, 9]
  
  # [a,b,c].transpose.map { |x| x.reduce :+ }
  
  # a more comprehensible solution[5]
end
```

```javascript
// I have a reason for using double equals.
if ( input == 1 ) {
  // do a thing.
}
```

We should want to push each other, and want to learn about the intricacies of the language - but not at the expense of 




---
1
2
3 - We can and will use static code formatters on anything that would need it -- it'll be ok.
4 - Sweetness and coolness are roughly analogous.
