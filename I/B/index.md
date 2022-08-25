### B. Create accessible JavaScript, AJAX, and interactive content.

Some of the highlights of accessible interaction design are shown in the list below (this list is NOT all-inclusive). 

1.  **Manage focus** - When JavaScript changes the visual focus (e.g. when a dialog is activated), JavaScript should be used to manage the keyboard focus so that it follows the visual focus.
2.  **Use semantic html** - HTML defines sets of elements, attributes, and attribute values. These features have specific semantic meanings and are intended to be processed by user agents in particular ways.
3.  **Consider DOM order when adding new content dynamically** - When content is added or altered on a page, it should generally be added after the current point of focus, because screen reader users are much less likely to navigate backward in the DOM than forward in the DOM, causing them to miss most additions/changes in previous positions in the DOM
4.  **Create device-independent event handlers** - JavaScript event handlers must be device-independent. The functionality must be available with the keyboard, mouse, touch, voice, etc.
5.  **Create accessible JavaScript widgets** - design patterns and examples of
    common widgets.
6.  **Simplify events** - Buttons and other interactive elements should generally have only one type of event associated with them. Multi-event elements are more difficult to make accessible and more difficult for users to understand. For example, either a menu item should act as a link or as a button that expands a submenu. Coding a menu item to expand the menu on hover and activate a link on click is problematic for keyboard users, touch users, and gesture-based mobile screen reader users.
