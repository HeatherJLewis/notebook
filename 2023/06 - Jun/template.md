# Learning CSS

Notes made from: [Steve Girffith's Learning CSS](https://www.youtube.com/watch?v=NZEz4yNITd8&list=PLyuRouwmQCjl4wTSNbb8RTKZuyMhoIxBe&index=5).

## CSS Padding and Margins

- collapses to the bigger amount for overlapping margins
- can target each margin individually
- can target each margin within the same line of values

## Box Model

- applied to every single element on the page
- content area
- 3 extra layers that can be added to the content area
- padding adds px to the content area
- border
- margin
- in the example below, the total width would be: 300 + 20 + 10 + 30 + 30 + 10 + 20 = 420px

```
p{
    height: 200px;
    width: 300px
    padding: 20px; /* same bg color as content area*/
    border: 10px solid red;
    margin: 30px; /* always transparent*/
}
```

Look at Steve's code [here](https://gist.github.com/prof3ssorSt3v3/4f43a28756743a123b89378bc1a08488).

- Can you work out what you would see in the browser after the CSS is applied?
- Why do you see the vertical spacing between paragraphs?
