# Creating Meaningful Links
Ensuring that your links and buttons has a concise and meaningful label, allows a screen reader user to discern what they are clicking on.  Most blind users will navigate your site by pulling up a list of elements, like links, which doesn't allow them to have the context around the link. For example, they will only hear 'Click here' opposed to the entire sentence (outside of the link) "to enroll in our class *__click here__*"

## Appropriate Use
### Concise and meaningful text
Links should have a concise and meaning text as in the examples below:
```html
<a href="/links.html"> Accessible Link </a>
```
Sometimes you may decide to use a button as a link. Buttons should be coded as buttons, and not as an image. You should avoid using images as links whenever possible. If you need to, the alt-text should all the user to know where that link takes them.

```html
<button type="submit"> Submit Form </button>
<a href="/home.html"> <img src="../path.jpg" alt="home"></a>
```

### Non-color indicators
We cannot use color only to convey meaning, and that includes indicating to your users that the text is a link with color only. The easiest way to achieve this is by underlining your links. 

Below are the WCAG requirements:
* A non-color indicator, such as an underline, must be present on hover
* The contrast ratio between the surrounding text and the background must be at least 4.5:1
* The contrast ratio between the link and the background must be at least 4.5:1
* The contrast ratio between the link and the surrounding text must be at least 3:1.


## How to test for compliance
We recommend using an automated checker like WebAIM's [WAVE Browser extension](https://wave.webaim.org/). This is available for Chrome, Firefox, and Edge browsers. When you click on the plug-in an overlay will appear with all of your issues.

In addition we recommend you:
1. Visually scan your site to ensure all links have non-color indicators
2. Use your tab key to ensure you can navigate to all your links. When doing so a *Focus-indicator* should appear. Depending on your browser this might be a red box around the link. If this does not appear, you will need to check your .CSS file.
3. Review the WAVE report to ensure there are no issues regarding your links. This may appear in either the "errors", "alerts", or "features" categories depending on the issue.


## Common Mistakes
### Read More, Click Here, More
**DO NOT** use Read More, or any similar verbage as the entire link. Instead phrase the whole link as 'Read more about our class of 2025'. The latter provides you the context to what the link is referring to, and what to expect when you click on it. 

### Buttons as images
Avoid using images as buttons on your page. Screen reader users navigate your site through the elements. This image will not appear in a list of buttons or links. 

### Adjacent Links
Pages should not present more than one link to the same destination next to each other. One common design pattern is for an image, a heading, and a word like “More” to each link to the same destination, such as in a news list. Assistive technology users may find navigating through several links a bad experience. Instead, provide one link. Either select one element to be the link, or wrap all elements within one link.

## Other resources
* [W3C Buttons and links](https://www.w3schools.com/accessibility/accessibility_buttons_links.php)

## WCAG Standards
* [WCAG 2.4.4: Link Purpose](https://www.w3.org/WAI/WCAG21/Understanding/link-purpose-in-context.html)

