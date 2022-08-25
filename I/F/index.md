# F. Create accessible single-page applications.
## Study topics related to single-page applications
1.  If the AJAX content is loaded as the direct result of a user action (e.g. activating a button), the screen reader user should be notified that new content has loaded. Methods that can be used to notify screen readers that new content has loaded include:

    a) Sending the focus to the new content

    b) Using aria-live to make an announcement without moving the focus.

2.  If the AJAX content is loaded passively (i.e. not as the direct result of a user action like activating a button), users may not need to be notified that the new content has loaded, depending on the importance and urgency of the content and whether the content has been inserted above the user's current position or not.
