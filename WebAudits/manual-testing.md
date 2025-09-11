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

#### Testing Method 1: Broswer Plug In 

<p>
<b> Tools used: </b><a href="https://wave.webaim.org/"> WAVE by WebAim </a> or <a href="https://opena11y.github.io/h2l-side-panel/"> Headings, Landmarks and Links</a> (H2L) browser plug-in <br>
<b> Testing instructions: </b> <br>
Launch the plug-in, and a panel should appear on the left side of your page. Headings will appear under the "Structure Tab" in Wave, and on the first tab, headings in the H2L tool. They will appear in the order that a screen reader will read them.
</p>

#### Testing Method 2: Screen Reader Verification
<b> Tools Used: </b> 
<ul>
  <li> <a href="https://www.nvaccess.org/download/"> NVDA </a> can be installed on any windows device.  </li>
  <li> <a href="https://portal.freedomscientific.com/SponsoredSoftware"> JAWS </a> can be installed from the freedom scientific website using your [at]rutgers.edu email address. </li>
  <li> VoiceOver comes preinstalled on all iOS and MacOS devices </li>
</ul>
Screen readers users will often jump to heading using their rotator or list of headings feature. They can also jump to next heading using a keyboard command. For the purposes of testing we'll use the rotator/list of headings feature so we can visually see all the headings and the order its read.

Select the screen reader you are using below. The instructions assumes you have launched the screen reader, and opened the page.
<details>
  <summary> NVDA - desktop testing </summary>
  <p> For optimaal results please conduct all test in Chrome <br>
    <table> 
      <tr>
        <th> Action </th>
        <th> Expected Results </th>
      </tr>
      <tr>
        <td> Caps Lock + F7  <br> 
            Insert + F7 </td> 
        <td> Opens an eleements list dialogue <sup> 1 </sup> </td>
      </tr>
          <tr>
        <td> Press Alt + H </td> 
        <td> This should put your focus on Headings radio button </td>
      </tr>
       <tr>
        <td> Press tab </td> 
        <td> This should put your focus list of headings </td>
      </tr>
      <tr>
        <td> Press the down arrow key </td> 
        <td> The screen reader should read out the heading and heading level. You can also visually see this in the list. </td>
      </tr>
    </table>
  Foot notes: <br>
  <ol>
    <li> When NVDA opens, it'll ask for your identifier key. By default Caps Lock will be checked. This option can be changed. If the menu does not open, try Insert + F7 instead. Additionally, if you hear "This feature is only available in a web document, like a page on the internet", then try refreshing the page. </li>
  </ol>
  </p>
</details>

<details>
  <summary> JAWS </summary>
  <p> For optimaal results please conduct all test in Chrome <br>
    <table> 
      <tr>
        <th> Action </th>
        <th> Expected Results </th>
      </tr>
      <tr>
        <td> Insert + F6 </td> 
        <td> Opens an eleements list dialogue <sup> 1 </sup> </td>
      </tr>
      <tr>
        <td> Press the down arrow key </td> 
        <td> The screen reader should read out the heading and heading level. You can also visually see this in the list. </td>
      </tr>
    </table>
   Foot notes: <br>
  <ol>
    <li> If you hear "This feature is only available in a virtual document, like a page on the internet", try refreshing the page. </li>
  </ol>
</details>

<details>
  <summary> VoiceOver </summary>
    <p> For optimaal results please conduct all test in FireFox <br>
    <table> 
      <tr>
        <th> Action </th>
        <th> Expected Results </th>
      </tr>
      <tr>
        <td> VO Key (Ctrl + Option) + U </td> 
        <td> Opens up your rotator <sup> 1 </sup> </td>
      </tr>
          <tr>
        <td> Press the right arrow key </td> 
        <td> The rotator will slide over to the list of headings. </td>
      </tr>
      <tr>
        <td> Press the down arrow key </td> 
        <td> The screen reader should read out the heading and heading level. You can also visually see this in the list. </td>
      </tr>
    </table>
   Foot notes: <br>
  <ol>
    <li> Your VO Key, which will be represented as just VO, is Ctrl + Option. If you hear "This feature is only available in a virtual document, like a page on the internet", try refreshing the page. </li>
  </ol>
</details>

#### Expected Results
  <ol> 
    <li> A H1 is present, and is the first heading on the page </li>
    <li> Headings follow a logical order, and is appropriately nested. For example you don't go from a H1 to a H3. </li>
    <li> There are no empty headings <sup>*</sup> </li>
    <li> The structure of the heading follow the intended outline of the page. For example the listed heading may put heading of names under founders, when the page refleccts visually they are teachers and under the teachers section. </li>
  </ol>
  &ast; Some plugins may not identify empty headings. It's important you are running an automated tool like <a href="https://wave.webaim.org/"> WAVE by WebAim </a> or doing screen reading testing for a complete testing experience. 
</p>
