# Full Manual Testing Guidelines

## Blindness
### Skip to Main is present and functions as expected
<p> The Skip to main allows for users to bypass the main navigation on the page, as they go through your website. </p>
**Tools Used:** Keyboard only <br>

**Testing instructions:** <br>
<table>
  <tr>
    <th> Action </th>
    <th> Expected Results </th>
  </tr>
  <tr>
    <td> Press <em>Tab</em> </td>
    <td> A hidden link should appear that reads Skip To Main, or Skip Navigation </td>
  </tr>
  <tr>
    <td> Press <em>Enter</em> </td>
    <td> The page should move to the main content on the page </td>
  </tr>
</table>

**Troubleshooting:** <br>
If you are using a CMS, this is often times built into the template file itself and you will need to work with your web developer to have them fix this issue.

### Appropriate Heading Structure
<p> Most blind users will navigate your site using the headings, or the Ctrl + F (find) function. </p>
<p>
<b> Tools used: </b> <a href="https://opena11y.github.io/h2l-side-panel/"> Headings, Landmarks and Links</a> browser plug-in <br>
<b> Testing instructions: </b> <br>
Launch the plug-in, and a panel should appear on the left side of your page. The first tab will display the headings in the order on the page.
</p>
<p>
<b> Expected Results: </b><br>
  <ol> 
    <li> A H1 is present, and is the first heading on the page </li>
    <li> Headings follow a logical order, and is appropriately nested. For example you don't go from a H1 to a H3. </li>
    <li> There are no empty headings <sup>*</sup> </li>
    <li> The structure of the heading follow the intended outline of the page. For example the listed heading may put heading of names under founders, when the page refleccts visually they are teachers and under the teachers section. </li>
  </ol>
  &ast; Some plugins may not identify empty headings. 
</p>
