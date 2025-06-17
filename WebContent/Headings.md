# Headings
Headingsare imporant, as it creates a structure that allows screen readers to navigate your site. It also improves the usability of your site, making it easy for viewers to find the information they need.

## Appropriate Use
### Code Example
You should use the appropriate heading tag, as outlined below. You can style these in your .CSS file to adjust the look and feel of each heading level
```html
  <h1> Main Topic </h1>
```

### Appropriately nest headings
Each heading should be appropriately nested as in the eample below, following a logical order.
```html
<h1> Main Topic </h1>
  <h2> Comparison </h2>
      <h3> Reason 1 </h3>
      <h3> Reason 2 </h3>
  <h2> Contrast </h2>

```

### Use concise Language
It's important as you lable your headings to use concise language. For example instead of a section being called 'How Students can enroll in our summer camp program' you can reword this to 'Enrolling in Summer Camp' 

## How to test for compliance
We recommend using the [Skip to Headings browser extension](https://chromewebstore.google.com/detail/skipto-landmarks-headings/fjkpbfcodhflpdildjbmdhhmcoplghgf?pli=1) on Google Chrome. This will allow you to visually see the heading structure on your page.

## Common Mistakes
### Empty Headers
A common mistake we see is when using a content management system, sometimes you may remove a header but the design tool as left a space where it was. This results in an empty heading. This will show up as [Empty Text Content] in the skip to headings plugin. 

![image](https://github.com/user-attachments/assets/640d6470-4bd1-4f53-b038-7656576393c4)

If you click on the empty link (in the Skip to Headings plugin) it will take you to that spot on the page, where you can view the code. It will likely look like the following:
```html
<h2>  <h2>
<p> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. </p>
```

### Improperly nested Headings
Using the plug you can also see where you may have improperly nested headings, for example going from H1 to H3. 

## Other resources
* [WebAim's creating semantic structure in Web content](http://webaim.org/techniques/semanticstructure/)

## WCAG Standards
* [WCAG 1.3.1: Info and Relationships](https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html)
* [WCAG 2.4.6: Headings and Labels](https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-descriptive.html)

