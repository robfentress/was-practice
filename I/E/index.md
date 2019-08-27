# E. Create interactive controls/widgets (standard or custom) based on accessibility best practices
## Study topics related to interactive controls/widgets
Some highlights of key concepts to take into account with interactive controls/widgets include the following (this list is NOT all-inclusive):
1. Become familiar with the keyboard interaction model with ARIA custom widgets. There are general keyboard patterns, plus keyboard patterns specific to types of widgets.

    a) In many widgets, the keyboard interaction model is to tab to the widget as a whole, or to the active/selected element within the widget, then use the arrow keys to navigate within the widget. The tab key is generally not used for navigation within the widget. Other keystrokes may be recommended for certain widgets.
2. Native HTML widgets should be used instead of custom WAI-ARIA widgets whenever possible, because of the built-in accessibility features of native HTML widgets. Implementing custom widgets requires greater attention to detail in the coding techniques and patterns, and support for custom widgets may vary, especially for less common widgets.
3. When creating ARIA widgets, pay attention to the semantic structure of the roles. Some roles have required parent or child roles, and some roles have required attributes.
4. When a custom role is assigned to an element, the custom role completely overrides the native role. For example, `<li role=”button”>` will be treated like a button by the accessibility API, not like a list item.
5. The application role should be used sparingly, if at all, because it overrides many assistive technology keystrokes, such as the keystrokes that allow screen reader users to navigate by semantic elements such as headings, landmarks, tables, etc.
