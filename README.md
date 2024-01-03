# What's this, then? 
It's a single-flile, HTML/CSS/JS flashcard/flipcard app designed to work in an HTML document in Blackboard Ultra LMS. 

## How do I customize it? 
The questions and answers live in an array of contants called `cards`. Here's the dummy/demo data

```
const cards = [
      {
        question: "What is the capital of France?",
        answer: "Paris",
      },
      {
        question: "What is the largest ocean in the world?",
        answer: "The Pacific Ocean",
      },
      {
        question: "What is the square root of 16?",
        answer: "4",
      },
    ];
```

## How do I deploy it?
1. In Blackboard Ultra, create a new Document.
2. Choose the `Add HTML` option.
3. Copy paste the contents of the `flashcard.html` file into the document.
4. Save.

 ## What remains to be done? 
 I'm still working on accessibility. 
