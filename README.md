# What's this, then? 
It's a single-file, HTML/CSS/JS flashcard/flipcard app designed to work in an HTML document in Blackboard Ultra LMS, though it should work in any LMS or any LMS or CMS where you have access to an HTML editor. And, of course, it will work in any web page where you have access to the code.  

## How do I customize it? 
The questions and answers live in an array of contants called `cards`. Here's the dummy/demo data. I've replaced the actual URLs for the images with something shorter, for simplicity. 

```
const cards = [
      {
        question: "What is the capital of France?",
        answer: "Paris",
        questionImage: "https://example.com/questionImage.jpg", 
        answerImage: "https://example.com/answerImage.jpg", 
      },
      {
        question: "What is the largest ocean in the world?",
        answer: "The Pacific Ocean",
        questionImage: "https://example.com/questionImage.jpg", 
        answerImage: "https://example.com/answerImage.jpg", 
      },
      {
        question: "What is the square root of 16?",
        answer: "4",
        questionImage: "https://example.com/questionImage.jpg", 
        answerImage: "https://example.com/answerImage.jpg", 
      },
    ];
```

## How do I deploy it?
1. In Blackboard Ultra, create a new Document.
2. Choose the `Add HTML` option.
3. Copy paste the contents of the `flashcard.html` file into the document.
4. Save.

## How do I make use of the xAPI features? 
The xAPI features are minimal and optional. If you want to take advantage of them, do the following:  
1. Sign up for an LRS at [SCORM Cloud](https://rusticisoftware.com/products/scorm-cloud/), [Veracity Learning](https://lrs.io/), etc.  
2. Copy the endpoint, username, and password values for your LRS into the relevant place in flashcard.html. 
3. Save and test. 

There are console.log statements in the code which will appear in the console telling you if the LRS connection is successful or not:  
* `LRS connection established`
* `Failed to set up LRS object` + error

You'll get one of these statements when the app attempts to send an xAPI statement: 
* `Failed to save async xAPI statement:` + response code
* `Async xAPI statement saved`

 ## What remains to be done? 
 - [ ] Improve accessibility
 - [ ] Implement more meaningful xAPI statements
 - [x] Implement basic xAPI
 - [x] Improve UX for display of long questions

 ## Learn More
 * TinCanJS docs: https://rusticisoftware.github.io/TinCanJS/
 * TinCanJS via jsDelivr CDN: https://www.jsdelivr.com/package/npm/tincanjs
