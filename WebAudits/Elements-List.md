#Types of Web Elements

## Menus
The W3C WAI has a tutorial on how menus should be used for navigation, included expected screen reader behavior. Please refer to the following pages:
* [Menu Tutorial](https://www.w3.org/WAI/tutorials/menus/)
  * [Structure](https://www.w3.org/WAI/tutorials/menus/structure/): Mark up menus in a way that reflects their structure and appropriately labels them.
  * [Styling](https://www.w3.org/WAI/tutorials/menus/styling/): Use commonly recognized design patterns to distinguish menus and the state of menu items.
  * [Fly-out Menus](https://www.w3.org/WAI/tutorials/menus/flyout/): Ensure fly-out (drop-down) submenus can be used appropriately by mouse and keyboard.
  * [Application Menus](https://www.w3.org/WAI/tutorials/menus/application-menus/): Add specific markup and keyboard behavior to resemble desktop application menus

### Expected Behavior
Source: https://www.w3.org/WAI/tutorials/menus/application-menus/#keyboard-behavior

<table>
  <caption> <b> Top Level Menu Items </b> </caption>
  <tr>
    <th> Key </th>
    <th> Action </th>
  </tr>
  <tr>
    <td> tab  </td>
    <td> Select the next focusable element outside of the menu. </td>
  </tr>
  <tr>
    <td> shift + tab </td>
    <td> Select the previous focusable element outside of the menu. </td>
  </tr>
  <tr>
  <td> right </td>
  <td> Select the next top-level menu item. </td>
  </tr>
  <tr>
<td> left </td>
    <td>  Select the previous top-level menu item. </td>
  </tr>
  <tr>
<td> return/enter <br>
  Space <br>
Down </td>
    <td> Open the submenu, select first submenu item. </td>
  </tr>
  <tr>
<td> up </td>
    <td> Open the submenu, select last submenu item. </td>
  </tr>
  <tr>
<td>  esc </td>
    <td> Leave the menu. </td>
  </tr>
</table>

<table>
    <caption> <b> Submmenu Items </b> </caption>
  <tr>
    <th> Key </th>
    <th>A ction </th>
  </tr>
  <tr>
    <td> tab </td>
    <td> Close the submenu, select the next focusable element outside of the menu. </td>
  </tr>
    <tr>
    <td>shift ⇧ + tab ⇥ </td>
    <td>  Close the submenu, select the previous focusable element outside of the menu. </td>
  </tr>
    <tr>
    <td> right</td>
    <td> Close the submenu, select the first item of the next top-level menu item. </td>
  </tr>
    <tr>
    <td> left </td>
    <td> Close the submenu, select the first item of the previous top-level menu item. </td>
  </tr>
    <tr>
    <td> return/enter <br> Spce </td>
    <td> Carry out function of this item. (In this example: bring up a dialog box with the text of the chosen menu item.) </td>
  </tr>
    <tr>
    <td> down </td>
    <td> Select next submenu item. </td>
  </tr>
    <tr>
    <td>up </td>
    <td> Select previous submenu item </td>
  </tr>
      <tr>
    <td> esc </td>
    <td> Close the submenu, select the current top-level menu item. </td>
  </tr> 
</table>



