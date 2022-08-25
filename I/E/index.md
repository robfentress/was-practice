# E. Create interactive controls/widgets (standard or custom) based on accessibility best practices
## Study topics related to interactive controls/widgets
Some highlights of key concepts to take into account with interactive controls/widgets include the following (this list is NOT all-inclusive):
1.  Become familiar with the keyboard interaction model for ARIA custom widgets. There are general keyboard patterns, plus keyboard patterns specific to types of widgets.
2.  In many widgets, the keyboard interaction model is to tab to the widget as a whole, or the active/selected element within the widget, then use the arrow keys to navigate within the widget. The tab key is generally not used for navigation within the widget. Other keystrokes may be recommended for certain widgets.
3.  Native HTML widgets should be used instead of custom WAI-ARIA widgets whenever possible, because of the built-in accessibility features of native HTML widgets. Implementing custom widgets requires greater attention to detail in the coding techniques and patterns, and support for custom widgets may vary, especially for less common widgets.
4.  When creating ARIA widgets, pay attention to the semantic structure of the roles. Some roles have required parent or child roles, and some roles have required attributes.
5.  When a custom role is assigned to an element, the custom role completely overrides the native role. For example, `<li role="button">` will be treated as a button by the accessibility API, not like a list item. <!-- We added the new items that were between 5 and 6 to the end of the lest, starting at 7 -->
6.  The application role should be used sparingly, if at all, because it overrides many assistive technology keystrokes, such as the keystrokes that allow screen reader users to navigate by semantic elements such as headings, landmarks, tables, etc.
7.  Roles to describe the type of widget presented, such as "menu", "treeitem", "slider", and "progressbar".
8.  Roles to describe the structure of the Web page that include headings, regions, and tables.
9.  Properties to describe the state widgets are in, such as "checked" for a checkbox, or "expanded" for a menu.
10. Properties to define live regions of a page that are likely to get updates (such as stock quotes), as well as an interruption policy for those updates---for example, critical updates may be indicated in an alert dialog box, and incidental updates occur within the page.
11. In the case of complex web applications or dynamic contents, ARIA roles, states, and properties may be used that communicate the screen reader with what is occurring in the interface.

