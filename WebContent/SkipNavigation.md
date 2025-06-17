# Skip Navigation
This is sometimes called Skip to Main. This allows a user to jump to the main content of the page, with out needing to read the heading and navigation on every page they click on. 

## Appropriate Use
Skip to Main is a hidden link that allows Screen-Readers to skip reading through the navigation bar every time they get to a new page and allows them to quickly jump to the main content.

There are several ways to do this, one way to add this to your site is to put this code after the body tag:
```html
    <body>
        <a href="#main" class="skip-to-main-content-link"> Skip to main content </a>
        ...
        ...
        <main id="main">
        ...
        </main>
    </body>
```

To hide this button off screen, you can add this line of code to your .css file

```html
    .skip-to-main-content-link {
        position: absolute;
        left: -9999px;
        z-index: 999;
        padding: 1em;
        background-color: black;
        color: white;
        opacity: 0;
      }
      .skip-to-main-content-link:focus {
        left: 50%;
        transform: translateX(-50%);
        opacity: 1;
      }
```

## How to test for compliance
When the page loads, you should press your *Tab Key*. An element should appear on the screen that reads 'Skip to Main' or 'Skip Navigation'
![image](https://github.com/user-attachments/assets/4d6174ac-25ad-4891-8196-f9cd95cf6c75)

It's important that you then click *enter* and ensure that the link does bring you to the main content

## Common Mistakes
### Link doesn't point to a location
A very common mistake we see is for a 'Skip to Nav' to exist in the template, but the end user has not identified the point on the page to link to. This creates a dead link on your page essentially. It's important that at the beginning of your  main content you are identifying id="main" for the link to work.

### Link takes you to the top of the page
This link should not bring you to the top of the page, as it then does not serve any purpose. It needs to bring you to a location after the main navigation.

## Other resources 
* [WebAIM: Skip Navgiation Link](https://webaim.org/techniques/skipnav/)

## WCAG Standards
* [WCAG 2.4.1: Bypass Blocks](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks)
