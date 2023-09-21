---
layout: essay
type: essay
title: "Coding Standards"
# All dates must be YYYY-MM-DD format!
date: 2023-09-20
published: true
labels:
  - Software Engineering
  - Coding Standards
  - JavaScript
---

Many people think about coding standards in trivial ways, such as space of indent or whether place the close-curly-brace on a new line. Those are partial understanding of coding standards. In fact, coding standards are absolutely more than that.Some people are big fans of coding standards and believe that if only one software engineering technique can be implemented to improve code quality, it should be a coding standard. I agree with that. The famous software engineer martin fowler said:

<p><em>"Any fool can write code that a computer can understand. Good programmers write code that humans can understand."</em></p>

So, why are coding standards important? As ordinary people, we all seem to be able to write code that makes computers run, but just because it runs doesn't mean it's high-quality code. In the actual workplace, one person can't write code that only one person can read. The readability of the code is important because the code may need to be evaluated, modified, or new features added after it is written. So code may be read far more often than it is run. Only by writing code that everyone can understand can we work together to better maintain the code. coding standards can help ensure the consistency of code and improve the readability of code. Second, coding standards act as a precautionary measure to help us detect basic anti-patterns and generic coding mistakes. And when these bugs or anti-patterns do occur, the code standard provides guidance on how to correct them. So coding standards are important, we have to first implement a set of coding standards and execute it, in order to lay a good foundation for other work.

I've use Intellij and ESlint for a week now. They impressed me. Before I met Intellij, I have used a lightweight IDE called JGrasp. JGrasp is simple and easy to learn to use, but it is not as powerful as Intellij, and it only shows errors until compile time, sometimes I write many lines of code and get a bunch of error messages after compilation. Unlike JGrasp, Intellij is a powerful and feature-rich IDE. And ESlint is a quality assurance tool for enforcing coding standards . The Intellij integred with ESlint helps me to examine code in real time as I write it and flag any errors. For some identified problems, it can also fix them automatically without manual changes. I also improved the understanding of coding standards by reading these error messages.Finding that getting a green check mark is painful, especially when I see those red wavy underlines on the screen. But at the same time, it's useful. I'm happy when I get a green check mark every time after I follow ESlint reminders because it's obvious that the code gets a green check mark is much cleaner than before. I think I should use them more and become familiar with them to make my code more standardized and readable.

