# Tables
Tables can be a powerful tool for organizing and presenting data. While sighted users can easily navigate the column and rows to find the information they need, screen reader users are not able to do the same with out headings appropriately tagged. 

## Appropriate Use
### Table Headings
You should always try to keep your tables simple, and avoid complex layouts. You should always ensure that you are using the *th* (Table Heading) tag to identify the heading rows or columns in your table, as in the example below:

```html
<table>
  <tr>
    <th>Date</th>
    <th>Event</th>
    <th>Venue</th>
  </tr>
  <tr>
    <td>12 February</td>
    <td>Waltz with Strauss</td>
    <td>Main Hall</td>
  </tr>
  […]
</table>
```


The WC3 provides great resources for how to code tables with:
* [Tables with one heading row or column](https://www.w3.org/WAI/tutorials/tables/one-header/)
* [Tables with 2 headings- rows and columns](https://www.w3.org/WAI/tutorials/tables/two-headers/)
* [Tables with irregular headers](https://www.w3.org/WAI/tutorials/tables/irregular/)
* [Tables with multi-level headers](https://www.w3.org/WAI/tutorials/tables/multi-level/)


### Captions and Summaries
Screen reader users are able to navigate your page through a list of elements, and this includes tables. This means they could jump to a table, and with out proper context (which you have provided in the text previous) they might not know that the table relates to. Having captions allow the user to understand what information is in the table.

For this we use the *caption* tag

```html
<table>
    <caption> Toyota Sales FY 2025 </caption>
    <tr>
        ....
</table>
```

For more complicated tables were a summary is required to describe how the information is laid out you can use the *span* tag to create text under the caption:

```html
<caption>Availability of holiday accommodation <br>
  <span>Column one has the location and size of accommodation, other columns show the type and number of properties available</span>
</caption>
```

## How to test for compliance
You will need to use an automated checker like WebAIM's [WAVE Browser extension](https://wave.webaim.org/). This is available for Chrome, Firefox, and Edge browsers. When you click on the plug-in an overlay will appear with all of your issues.

You can also use the developer tools in your browser to select the headings and ensure they have the *th* tag.

## Common Mistakes
### Using tables to style your page
**DO NOT** use tables as way of styling the layout of your page. Instead use CSS to [create grid layouts](https://www.w3schools.com/css/css_grid.asp). This is a lot more usable for the end user, and will reflow (if done correctly) when the page is enlarged or viewed on smaller devices. 

## Other resources
* [W3C Table Tutorial](https://www.w3.org/WAI/tutorials/tables/)
* [WebAim Accessible Tables](https://webaim.org/techniques/tables/data)

## WCAG Standards
* [WCAG 1.3.1 Info and Relationships](https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html)