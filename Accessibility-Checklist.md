# :heart: Accessibility Checklist

Working Definition of Accessibility: 

Ensuring everyone, regardless of physical or mental characteristics, is able to use an application.

### What accessibility gaps are you targeting, especially for your application's user base?

This info is useful in prioritizing what to do *first*.

* Cognitive 
* Physical
* Auditory
* Visual

[Read explanations and examples of abilities and barriers here.](https://www.w3.org/WAI/people-use-web/abilities-barriers/)

## Recommended: Easier Accessibility Enhancements

Click links for further reading on an enhancement.

* [Headings](https://accessibility.iu.edu/creating-content/web-content/headings.html) - Content should be broken up by headings in `h` elements to make pages easy to navigate/scan
* [Meaningful, Descriptive Link Text](https://webaim.org/techniques/hypertext/link_text) - Don't use meaningless phrases like "Click Here" for your link text, it should describe what the link actually goes to
* [Semantic, Valid HTML](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML) - Minimize use of meaningless `div` and `span` elements, use semantic elements like `section` or `nav` instead. Make sure your HTML validates to modern specs
* [Font Size & Readability](https://webaim.org/techniques/fonts/) - Unofficial mininum 16px font size for body text, but also watch out for your text readability dependent on styling
* [Color Contrast Ratio](https://webaim.org/articles/contrast/) - 4.5:1 minimum contrast ratio, though aim for better. Ensure your text color isn't too close to your background color, making it hard to read. Some exceptions apply for large text
* [Alt Tags on Images](https://www.w3.org/WAI/tutorials/images/tips/) - All images should have `alt` tags filled out describing the purpose of the image
* [Large Click Targets](https://www.a11yproject.com/posts/2018-11-21-large-touch-targets) - 44px by 44px minimum size for clickable things, with a few exceptions such as inline text links
* [Remove Images Of Text](https://accessibility.princeton.edu/how/content/images-text) - Use actual HTML text instead of using an image of text--text in images cannot be understood by assistive technologies
* [Don't Hide Focus Indicator](https://web.accessibility.duke.edu/learn/focus-indicator) - It's possible to remove/override the default browser focus indicator with the CSS `:focus` pseudo element or `outline: 0;` style, which can make it difficult to see what element is active

## Higher Effort Accessibility Enhancements

* [Zoom](https://usability.yale.edu/web-accessibility/articles/zoom-resizing-text) - Layout doesn't break and content stays visible when zooming using browser, allows zooming to 200%+
* [Keyboard Navigation](https://www.nngroup.com/articles/keyboard-accessibility/) - User can use essential functions--especially forms--and navigate page with keyboard, not getting stuck on an element
* [WAI-ARIA attributes](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/WAI-ARIA_basics) - Used to describe elements and states to accessibility software
* [Limiting animation/motion](https://css-tricks.com/accessible-web-animation-the-wcag-on-animation-explained/) - Minimize use of animation, allow user to control/disable if animation is used
* Video captions - Full text captions and transcripts for video content
* [Fully semantic elements and information structure](https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-sequence.html) - Content is organized intuitively, sensibly, in understandable chunks for both humans and assistive technologies with all parts using meaningful elements
* [Increase readability, simplify language](https://css-tricks.com/accessible-web-animation-the-wcag-on-animation-explained/) - Complex, long sentences and words can create issues with reading and understanding your content, especially for users with disabilities
* [Don't Rely On Only Color as a Differentiator](https://www.smashingmagazine.com/2016/06/improving-color-accessibility-for-color-blind-users/) - Colorblind users can have difficulty differentiating items solely based on color. Sometimes items are only color coded in your user interface. Items should have another differentiator such as an icon or descriptive text as a backup

## Resources

* [Automated Web Accessibility Evaluation Tool](https://wave.webaim.org/)
* [Low Hanging Fruit of Web Accessibility](https://kb.rice.edu/page.php?id=93992#fruit)
* [Accessibility Tools Listing from the W3C](https://www.w3.org/WAI/ER/tools/)
* Lighthouse - Auditing tool integrated in Chrome DevTools checks for some accessibility compliance issues
* [W3C Acccessibility Training](https://www.edx.org/course/web-accessibility-introduction) - Official and free accessibility training from the W3C, the governing body of web standards
* [Accessibility Checklist](https://www.a11yproject.com/checklist) - Good accessibility checklist by these well known accessibility advocates
