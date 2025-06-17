# ARIA Landmarks
A common way of many screen reader users to navigate your site, is through the landmarks. These are regions that you have created on your page. We achieve this using a combination of HTML5 and ARIA labels. ARIA is used to provide instructions to assistive technology, letting them how to identify, read out, or interact with an element.

## Appropriate Use
It is recommended that you start with using HTML 5 semantic regions. These are the following: 
```html
<header>, <nav>, <main>, <section>, <aside>, <footer>
```
These should correspond to the regions on your page:

![image](https://github.com/user-attachments/assets/ae9dd2ea-1d98-49da-b961-1ef5e106f56a)

It is common for you to have multiple navigation, sections, and sometimes side items. For these it's important that you are providing a usable label so that the end user can discern one element from the other. 

In the example below we've code two navigation items
```html
<nav aria-label="Main Navigation"> ... </nav>
...
<nav aria-label="Book Chapters"> ... </nav>
```

The same method of aria-label="text" can be applied to the sections and aside items:

```html
<section aria-label="Your text here"> ... </section>
 <aside aria-label="Your text here"> ... </aside>
```

## How to test for compliance
We recommend using the [Skip to Headings browser extension](https://chromewebstore.google.com/detail/skipto-landmarks-headings/fjkpbfcodhflpdildjbmdhhmcoplghgf?pli=1) on Google Chrome. This will allow you to visually see the landmark structures on your page.

## Common Mistakes
### Not labeling landmarks
A very common mistake we see, is not providing an ARIA label to your sections. This results in the screen reader listing:
  * Navigation
  * Navigation
  * Complimentary Region
  * Complimentary Region
  * Complimentary Region
  
 This does not provide any usable information that allows the user to navigate your site


## Other resources
* [W3C ARIA Landmark Examples](https://www.w3.org/WAI/ARIA/apg/patterns/landmarks/examples/main.html)
* [Using Landmarks to identify regions](https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-descriptive.html)

## WCAG Standards
* [WCAG 1.3.1: Info and Relationships](https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html)
* [WCAG 2.4.6: Headings and Labels](https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-descriptive.html)
* 
