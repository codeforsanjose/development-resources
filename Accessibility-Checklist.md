# Accessibility Checklist

Working Definition of Accessibility: 

Ensuring everyone, regardless of physical or mental characteristics, is able to use an application.

### What accessibility gaps are you targeting, especially for your application's user base?

This info is useful in prioritizing what to do *first*.

* Cognitive 
* Physical
* Auditory
* Visual

[Read explanations and examples of abilities and barriers here.](https://www.w3.org/WAI/people-use-web/abilities-barriers/)

# Recommended: Easier, But High Value Accessibility Enhancements

* [Headings](https://accessibility.iu.edu/creating-content/web-content/headings.html) - Content should be broken up by headings in `h` elements to make pages easy to navigate/scan
* [Meaningful, Descriptive Link Text](https://webaim.org/techniques/hypertext/link_text) - Don't use meaningless phrases like "Click Here" for your link text, it should describe what the link actually goes to
* [Semantic HTML](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML) - Minimize use of meaningless `div` and `span` elements
* [Font Size & Readability](https://webaim.org/techniques/fonts/) - Unofficial mininum 16px font size for body text, but also watch out for your text readability dependent on styling
* [Color Contrast Ratio](https://webaim.org/articles/contrast/) - 4.5:1 minimum contrast ratio, though aim for better. Ensure your text color isn't too close to your background color, making it hard to read. Some exceptions apply for large text
* [Alt Tags on Images](https://www.w3.org/WAI/tutorials/images/tips/) - All images should have `alt` tags filled out describing the purpose of the image
* [Large click targets](https://www.a11yproject.com/posts/2018-11-21-large-touch-targets) - 44px by 44px minimum size for clickable things, with a few exceptions such as inline text links

# Harder Accessibility Enhancements

* Zoom - Layout doesn't break when zooming, allows zooming to 200%+
* Keyboard Navigation - User can use essential functions and navigate page with keyboard, not getting stuck on an element
* WAI-ARIA attributes - Used to describe elements and states to accessibility software
* Limiting animation/motion - Minimize use of animation or allow user to control if animation is used
* Video captions - Full text captions and transcripts for video content
* [Fully semantic page structure and content flow](https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-sequence.html) - Content is organized in a way that can be flowed through in a way that makes sense by assistive technologies with all parts using meaningful elements

# Resources

* [Automated Web Accessibility Evaluation Tool](https://wave.webaim.org/)
* [Low Hanging Fruit of Web Accessibility](https://kb.rice.edu/page.php?id=93992#fruit)
* [Accessibility Tools Listing from the W3C](https://www.w3.org/WAI/ER/tools/)
* Lighthouse - Auditing tool integrated in Chrome DevTools checks for some accessibility compliance issues
* [W3C Acccessibility Training](https://www.edx.org/course/web-accessibility-introduction) - Official and free accessibility training from the W3C, the governing body of web standards
* [Accessibility Checklist](https://www.a11yproject.com/checklist) - Good accessibility checklist by these well known accessibility advocates
