# Color Contrast
Color is a powerful design tool, helps convey meaning, and draws attention to content. It must be used thoughtfully so it does not present a barrier to people with disabilities, such as those who are colorblind, have low vision, or use grayscale monitors.

## Appropriate Use
### Text on a sold background
The Web Content Accessibility Guidelines require that text - and images of text - provide a contrast ratio of at least 4.5:1. This is ratio between the foreground and background colors.

### Non-text elements
For all other elements like buttons, images, links, form fields, etc the same rules regarding color contrast apply.

## How to test for compliance
You will need to use an automated checker like WebAIM's [WAVE Browser extension](https://wave.webaim.org/). This is available for Chrome, Firefox, and Edge browsers. When you click on the plug-in an overlay will appear with all of your issues.

When using an automated checker it is possible to get false positives, inwhich case you will need to manually verify that they are true issues.

Additionally, you should check any text in images, and any text above an image (like a call out in a hero banner). 

## Common Mistakes
### Links
A common mistake we see often is the color of hyperlinks on your page. In many cases this is set on in the .css as part of the template, and used against multiple backgrounds with out consideration to all those new colors. 

See the Rutgers [Color Contrast Look up](https://jkhurdan.github.io/A11yTraining/WebContent/ColorFilter.html) for which color combinations meet standards

## Other resources

## WCAG Standards
* [1.1.1 Non-text Content](https://www.w3.org/WAI/WCAG21/quickref/#qr-text-equiv-all)
* [1.4.1 Use of Color](https://www.w3.org/WAI/WCAG22/Understanding/use-of-color.html)
* [1.4.3 Contrast (Minimum)](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum) 
* [1.4.11 Non-text Contrast](https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html)
