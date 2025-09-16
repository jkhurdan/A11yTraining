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

<hr> 


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
  <summary> JAWS - desktop testing </summary>
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
  <summary> VoiceOver - desktop testing </summary>
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
    <li> The structure of the heading follow the intended outline of the page. For example the listed heading may put headings of names under founders, when the page refleccts visually they are teachers and under the teachers section. </li>
  </ol>
  &ast; Some plugins may not identify empty headings. In our experience <a href="https://wave.webaim.org/"> WAVE by WebAim </a> will identify those issues. 
</p>
<hr>

### Landmarks are apporpriately defined
<p> Landmarks allow a blind users to jump between sections on a page </p>

#### Testing Method 1: Broswer Plug In 
<p>
<b> Tools used: </b> <a href="https://opena11y.github.io/h2l-side-panel/"> Headings, Landmarks and Links</a> (H2L) browser plug-in <br>
<b> Testing instructions: </b> <br>
Launch the plug-in, and a panel should appear on the left side of your page. Landmarks will appear on the second tab in the H2L tool. They will appear in the order that a screen reader will read them.
</p>

#### Testing Method 2: Screen Reader Verification
<b> Tools Used: </b> 
<ul>
  <li> <a href="https://www.nvaccess.org/download/"> NVDA </a> can be installed on any windows device.  </li>
  <li> <a href="https://portal.freedomscientific.com/SponsoredSoftware"> JAWS </a> can be installed from the freedom scientific website using your [at]rutgers.edu email address. </li>
  <li> VoiceOver comes preinstalled on all iOS and MacOS devices </li>
</ul>
Screen readers users will often jump to landmarks using their rotator or list of landmarks feature. They can also jump to next landmark using a keyboard command. For the purposes of testing we'll use the rotator/list of landmarks feature so we can visually see all the headings and the order its read.

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
        <td> Press Alt + D </td> 
        <td> This should put your focus on Landmarks radio button </td>
      </tr>
       <tr>
        <td> Press tab </td> 
        <td> This should put your focus list of Landmarks </td>
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
        <td> Insert + Crtl + ; (semicolon)</td> 
        <td> Opens a list of landmarks on the page </td>
      </tr>
      <tr>
        <td> Press the down arrow key </td> 
        <td> The screen reader should read out the heading and heading level. You can also visually see this in the list. </td>
      </tr>
    </table>
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
        <td> Press the right arrow key until you get to the landmarks menu </td> 
        <td> The rotator will slide over to the list of landmarks </td>
      </tr>
      <tr>
        <td> Press the down arrow key </td> 
        <td> The screen reader should read out each landmark on the page. You can also visually see this in the list. </td>
      </tr>
    </table>
   Foot notes: <br>
  <ol>
    <li> Your VO Key, which will be represented as just VO, is Ctrl + Option. If you hear "This feature is only available in a virtual document, like a page on the internet", try refreshing the page. </li>
  </ol>
</details>

#### Expected Results
  <ol> 
    <li> A Navigation and Main landmark is present </li>
    <li> Landmarks have usable labels, that descern what they are </li>
  </ol> 
</p>
<hr>

### Tab Key Test 1: Menu Test
This test will ensure that a user with a screen reader can navigate through your manu with out issue.

#### Testing Method 1: Tab Key only 
<p>
<b> Tools used: </b> Tab Key <br>
<b> Testing instructions: </b> <br>
Press your tab key to ensure that you are able to navigate to the menu, read all of the menu items, including accessing any submenus. 
</p>

<hr>




## Low Vision

### Menu Collapsed and Usable
<b> Tool Used: </b> Browser zoom in function <br>
<p>
<b> Testing Instructions: </b> <br>
While WCAG Requires users to test at 200%, most low vision users we have encountered will increase the page between 350%-400%. As such you will encrease your browser to 400%. As some screens are larger than others, you will also adjust the size of your window to half the wiidth of your screen. </p>
<p>

<b> Expected Results: </b> <br>
* The menu should collapse, and there should be a hamburger menu that allows you to open the menu
* All items in the menu should be readable, and they should not break the page (letters shouldn't be cut off in the words). For example if the link title read "Understanding the Geopolitics between North and South Dakota", and now the link just reads "Understanding the geop"
* The menu item is still visually readable, and there are no contrast errors presented as a result of the page change
</p>
<hr>

### Page Reflowed correclty, and all contents are still readable 
<b> Tool Used: </b> Browser zoom in function <br>
<p>
<b> Testing Instructions: </b> <br>
While WCAG Requires users to test at 200%, most low vision users we have encountered will increase the page between 350%-400%. As such you will encrease your browser to 400%. As some screens are larger than others, you will also adjust the size of your window to half the wiidth of your screen. </p>
<p>

<b> Expected Results: </b> <br>
* All of items on the page should have reflowed including the menu, and there shouldn't be any text cut off on the page
* Images should still be present and should not be cut off on the page
* There shouldn't be any items obstructing the page. For example sometimes there's a notification bar or header that has a fixed position that will obstruct the text on the page.
</p>
<hr>

### Color Contrast Verified 
<b> Tool Used: </b> <a href="https://wave.webaim.org/"> WAVE by WebAim </a> <br>
<p>
<b> Testing Instructions: </b> <br>
Open WAVe by webaim, and proceed to the Contrast tab. You will need to use the Color Picker tool to verify all of the issues it has identified.  </p>
<p>

<b> Expected Results: </b> <br>
* All of items on the page should meet WCAG 2.1 AA standards
</p>
<hr>

### Keyboard Traps 
<b> Tool Used: </b> Browser zoom in function <br>
<p>
<b> Testing Instructions: </b> <br>
While WCAG Requires users to test at 200%, most low vision users we have encountered will increase the page between 350%-400%. As such you will encrease your browser to 400%. As some screens are larger than others, you will also adjust the size of your window to half the wiidth of your screen.
</p>
<p> From here you are going to tab through your menu, and hit the esc key to close it. Proceed to do this for any item that appears in a module or pop up, like chat bots, images, warnings/alerts, etc. </p>
<p>

<b> Expected Results: </b> <br>
* Items should close when using the esc key
</p>
<hr>

## d/Deaf and Hard of Hearing

### Closed Captioning on Videos
<b> Tool Used: </b> N/a <br>
<p>
<b> Testing Instructions: </b> <br>
Review the page to find any videos that are embeded inside the page. Videos may have open captions - which is text that is embeded in the video, or closed captions- which is a file that you can turn on and off, and overlays ontop of the video.  </p>
<p>

<b> Expected Results: </b> <br>
* The captions should match what is being said and use appropriate grammar and punctuation to convey intended meaning (i.e “Let’s eat, Grandma” vs. “Let’s eat Grandma”).
* Captions shoudl appropriately sync with when the audio happens
* Includes a completed textual representation of the audio, including speaker identification and non-spech information. This includes denoting sounds that are important (i.e melodic music)
* Captions should have a minimum duration of 40 frames (~1.5 seconds) and a maximum duration of 6 seconds. Background music notation is an exception to this guideline.
* Transcripts, unlike captions, are not always synchronized with audio content. For items like podcasts, TED Talks, interviews, or other mediums where there aren’t a lot of additional movement and sounds that need to be referenced, a transcript could be an acceptable media alternative.
* Captions (especially open captions) should have sufficent constrast between the text and the background. 
</p>
<hr>
