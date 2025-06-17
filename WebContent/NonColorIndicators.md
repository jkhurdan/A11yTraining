# Alternatives to Color to Convey meaning
It's important that you are not using color only to convey meaning. This can be done through the use styling (like underlining links), use of patterns, and the addition of text to describe intent.

## Appropriate Use
### Use of Text to convey meaning
Below we use color and text to signify dates with available tickets. 
<table>
 <tr>
  <th> Status </th>
  <th> Event Date </th>
  <th> Description </th>
 </tr>
 <tr>
  <td bgcolor="red"> Closed </td>
  <td> 9/21/25 </td>
  <td> Team A vs Team B </td>
 </tr>
 <tr> 
 <td bgcolor="green"> Open </td>
 <td> 9/27/25 </td>
 <td> Team A vs Team C </td>
 </tr>
</table>

### Accessible Links
We cannot use color only to convey meaning, and that includes indicating to your users that the text is a link with color only. The easiest way to achieve this is by underlining your links. 

Below are the WCAG requirements:
* A non-color indicator, such as an underline, must be present on hover
* The contrast ratio between the surrounding text and the background must be at least 4.5:1
* The contrast ratio between the link and the background must be at least 4.5:1
* The contrast ratio between the link and the surrounding text must be at least 3:1.


## How to test for compliance
We recommend using an automated checker like WebAIM's [WAVE Browser extension](https://wave.webaim.org/). This is available for Chrome, Firefox, and Edge browsers. When you click on the plug-in an overlay will appear with all of your issues.

You may have to manually check images with text as these will not be scanned with the automated checker. 


## Common Mistakes
### Using Color in images to convey meaning
A common mistake we see are images that use color only to convey meaning. This could include Bar Charts or other graphics. Consider the use of patterns in addition to the use of color.

### Color Contrast of text in images
If there is text on top of an image, please use WebAim's [Color Contrast Checker](https://webaim.org/resources/contrastchecker/) to manually check that the color of the text meets standards. In some cases you may need to check multiple places on the image. 

Please note, automated checkers will not pick up this issue. You will need to manually check these items. We recommend you avoid using text on top of images. 


## Other resources
* [W3C- Colors with Good Contrast](https://www.w3.org/WAI/perspective-videos/contrast/)

## WCAG Standards
* [1.1.1 Non-text Content](https://www.w3.org/WAI/WCAG21/quickref/#qr-text-equiv-all)
* [1.4.3 Contrast (Minimum)](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum) 