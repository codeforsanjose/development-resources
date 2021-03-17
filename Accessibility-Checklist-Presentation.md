## Background

* Practical, actionable, short checklist for busy developers
* Low hanging fruit for immediate accessibility gains
* Perfect is the enemy of done--incremental improvements are more likely to implemented
* Not meant to be comprehensive
* Not a substitute for a full accessibility audit
* Living document--work in progress, open to improvements/contributions
* https://github.com/codeforsanjose/development-resources/blob/main/Accessibility-Checklist.md

































## What Is Accessibility?

*Working Definition of Accessibility:*

Ensuring everyone, regardless of physical or mental characteristics, is able to use an application.

### Rationale

* Definitions are important to get teams working off the same basic assumptions
* Not everyone knows or has experience with web accessibility







































## Know Your Audience

What accessibility gaps are you targeting, especially for your application's user base?

This info is useful in prioritizing what to do *first*.
* If you can't fix everything, what is most important to fix first for your audience?

Examples:

* Cognitive - ADHD, memory impairment, seizures/sensitivity to flickering
* Physical - Missing fingers, arthritis, tremors/spasms 
* Auditory - Mild hearing impairment, deafness
* Visual - Colorblindness, low visual acuity, blindness







































## (Relatively) Easier Accessibility Enhancements


























## Headings

Content should be broken up by headings in h elements to make pages easy to navigate/scan

```
<h1>Project Report</h1>

<p>This was a cool project</p>
<p>Here's my introduction and summary</p>

<h2>Section 1</h2>

<p>Excellent progress</p>
```






































## Meaningful, Descriptive, Obvious Links & Text 

Don't use meaningless phrases like "Click Here" for your link text, it should describe what the link actually goes to. Also make sure links/clickable things are obvious.

```
<p>
Chips are a very crunchy food, though some people argue it's actually crispy. 
These 2 schools of thought frequently clash, <a href="https://chipsnodip.com">this article goes over the debate spanning 100 years</a>
</p>

...

<a class="button">
  Download Statistical Report
</a>
```







































## Semantic, Valid HTML 

Minimize use of meaningless div and span elements, use semantic elements like section or nav instead. Make sure your HTML validates to modern specs

```
NO:

<div>
   <div>
      <div>Home</div><div>Contact</div><div>About</div>
   </div>
   <div>
   Some Title
   </div>
   <div>
      This is the description. Oh look here's a button: 
      <div><div>$</div>Download Files</div>
   </div>
   <div>
      <applet code="javainthebrowser.class"></applet>
      <frame>Wow 2 pages in one!</frame>
   </div>
</div>

YES:

<nav>
  <button>About</button>
  <button>Contact</button>
</nav>
<main>
  <section>
    <h1>Here Ye Here Ye</h1>
    <p>I declare a thumb war</p>
  </section>
</main>
<footer>
  <p>Copyright 40,000 Adeptus Mechanicus</p>
</footer>
```











































## Font Size & Readability

Unofficial mininum 16px font size for body text, but also watch out for your text readability dependent on styling


```
NO:
p {
  /* Small text looks super sophisticated! */
  font-size: 6px;
}

<p>No one can read this!</p>

```

















































## Color Contrast Ratio

4.5:1 minimum contrast ratio, though aim for better. Ensure your text color isn't too close to your background color, making it hard to read. Some exceptions apply for large text

```
NO:

body {
  background: white;
  /* Light gray text on a white background is the pinnacle of class and elegance */
  color: #ccc;
}

<p>Strain your eyes to read this please; I detest eyes.</p>

```








































## Alt Tags on Images

All images should have alt tags filled out describing the purpose of the image

```
<img src="cat-doing-taxes.jpg" alt="Illustrates the proper method for a short hair cat to do your taxes" />
```


































## Large Click Targets

44px by 44px minimum size for clickable things, with a few exceptions such as inline text links

```
NO:

button {
  /* We hate people cancelling our Very Important Service (TM)  */
  width: 2px;
  height: 1px;
}

<button>Cancel</button>
```





























## Remove Images Of Text

Use actual HTML text instead of using an image of text--text in images cannot be understood by assistive technologies

```
NO:

<img src="SPIDERS_TITLE_TEXT.png" />

YES:

<h1>SPIDERS! The Musical</h1>
```

































## Don't Hide Focus Indicator

It's possible to remove/override the default browser focus indicator with the CSS :focus pseudo element or outline: 0; style, which can make it difficult to see what element is active

```
a, a:focus {
  /* It looks ugly when people can see what their keyboard is selecting, nuke it! */
  outline: none;
}

<a href="/action">Will this be visited when you press enter? It's a surprise!</a>
```





































## Higher Effort Accessibility Enhancements

## Zoom
Layout doesn't break and content stays visible when zooming using browser, allows zooming to 200%+

## Keyboard Navigation
User can use essential functions--especially forms--and navigate page with keyboard, not getting stuck on an element

## WAI-ARIA attributes
Used to describe elements and states to accessibility software

## Limiting animation/motion
Minimize use of animation, allow user to control/disable if animation is used

## Video captions 
Full text captions and transcripts for video content

## Fully semantic elements and information structure
Content is organized intuitively, sensibly, in understandable chunks for both humans and assistive technologies with all parts using meaningful elements

## Increase readability, simplify language
Complex, long sentences and words can create issues with reading and understanding your content, especially for users with disabilities

## Don't Rely On Only Color as a Differentiator
Colorblind users can have difficulty differentiating items solely based on color. Sometimes items are only color coded in your user interface. Items should have another differentiator such as an icon or descriptive text as a backup








































## View the Checklist

https://github.com/codeforsanjose/development-resources/blob/main/Accessibility-Checklist.md
