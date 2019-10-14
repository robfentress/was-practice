# Study Tasks
Below are the stated (and sometimes inferred) study tasks from the [WAS Body of Knowledge (BOK) document](https://iaap.membershipsoftware.org/files/IAAP%20WAS%20BOK%202_0_1019.docx), numbered for easier reference.
## [I. Create Accessible Web Content (40%)](I/index.md)

### A. Understand and interpret accessibility specifications and techniques
1. Understand and interpret WCAG 2
    
    a) Understand the relationship between principles, guidelines, success criteria, and their related success/failure techniques. ([questions for I:A.1.a](I/A/1.a.gift))

    b) Understand the intent, requirement, and impact of each principle, guideline, and success criterion.

    c) Be familiar with sufficient, failure, and advisory techniques for each success criterion.

    d) Understand the conformance level designations (A, AA, AAA).

    e) Identify the conformance level of each WCAG 2 success criterion. 

    f) Understand the three types of techniques and the W3C vetting process for techniques.
2. Understand and interpret WAI-ARIA 1

    a) Understand the purpose and impact of WAI-ARIA. 

    b) Understand the WAI-ARIA model of names, roles, and values.

    c) Know when and why to user WAI-ARIA, and when to use standard HTML instead.

    d) Be familiar with the authoring practices for custom widgets, including semantic structure, keyboard behavior, etc.
3. Understand and interpret ATAG 2

    a) Understand how ATAG 2 applies to web sites.

    b) Understand the meaning and intent of the two main sections of ATAG 2.

    c) Understand the intent, requirement, and impact of each principle, guideline, and success criterion.

    d) Distinguish between good automated practices in authoring tools and good practices that require author/user input

    e) Understand the power and limitations of automated accessibility authoring features
4.	Understand the difference between normative and non-normative documents and information, and be able to identify which documents are normative.

### B. Create accessible JavaScript, AJAX, and interactive content.
Some of the highlights of accessible interaction design are shown in the list below (this list is NOT all-inclusive). 
1. **Manage focus** - When JavaScript changes the visual focus (e.g. when a dialog is activated), JavaScript should be used to manage the keyboard focus so that it follows the visual focus.
2. **Use semantic html** - HTML defines sets of elements, attributes, and attribute values. These features have specific semantic meanings and are intended to be processed by user agents in particular ways.
3. **Keep content and its changes perceivable** - When content is added or altered on a page, it should generally be added after the current point of focus, because screen reader users are much less likely to navigate backward in the DOM than forward in the DOM, causing them to miss most additions/changes in previous positions in the DOM
4. **Create device-independent event handlers** - JavaScript event handlers must be device-independent. The functionality must be available with the keyboard, mouse, touch, voice, etc.
5. **Consider DOM order when adding new content dynamically**: When content is added or altered on a page, it should generally be added after the current point of focus, because screen reader users are much less likely to navigate backward in the DOM than forward in the DOM, causing them to miss most additions/changes in previous positions in the DOM.
6. **Simplify events** - Buttons and other active elements should generally have only one type of event associated with them. Multi-event elements are more difficult to make accessible, and more difficult for users to understand. For example, a menu item should either act as a link or as a button that expands a submenu. Coding a menu item to expand the menu on hover and activate a link on click is problematic for keyboard users, touch users, and gesture-based mobile screen reader users.

### C. Integrate accessibility into the quality assurance process.
Study topics related to accessibility quality assurance
1. Characterize and differentiate between the disciplines of Agile and Waterfall project management methodologies, and compare the approaches each methodology would have in relation to accessibility quality assurance.
2. Demonstrate an understanding of the benefits of designing digital content with accessibility in mind as opposed to remediation.
3. Characterize and differentiate between the disciplines of accessibility and user experience design, and compare assumptions of each discipline. 
4. Demonstrate an understanding of user testing, and compare to accessibility verification testing (AVT).
5. Understand how accessibility needs to be integrated into the entire product life cycle, including concept, requirements, design, prototyping, development, quality assurance (QA), user acceptance testing (UAT), and regression testing.
6. Identify ways in which each person’s role in the product life cycle can include some aspect of accessibility.

### D. Choose accessibility techniques that are well-supported
Study topics related to accessibility support
1. Understand the importance of coding to standards, rather than to the quirks or features of only one set of technologies.
2. Understand the concept of progressive enhancement, in which the baseline interaction is possible using old browsers and assistive technologies, and the more modern web site features are available for more modern browsers and assistive technologies.
3. Understand the importance of testing web designs for accessibility across a variety of platforms, browsers, and assistive technologies, and not just assuming they’ll work, even if they technically conform to published accessibility specifications.
4. Know which combinations of assistive technologies work best with which browsers, for testing purposes.
5. Know how to determine when an inaccessible outcome is the result of poor design versus poor technology support. 
6. Know how to tell the difference between inaccessible content and incomplete or faulty accessibility testing techniques.
7. Avoid design techniques or technologies that work only on certain platforms.
8. Know when it may be appropriate to write code that overrides, supplements, or fixes bugs in browsers or assistive technologies (do this only with great caution!).

### E. Create interactive controls/widgets (standard or custom) based on accessibility best practices
Study topics related to interactive controls/widgets
Some highlights of key concepts to take into account with interactive controls/widgets include the following (this list is NOT all-inclusive):
1. Become familiar with the keyboard interaction model with ARIA custom widgets. There are general keyboard patterns, plus keyboard patterns specific to types of widgets.

    a) In many widgets, the keyboard interaction model is to tab to the widget as a whole, or to the active/selected element within the widget, then use the arrow keys to navigate within the widget. The tab key is generally not used for navigation within the widget. Other keystrokes may be recommended for certain widgets.
2. Native HTML widgets should be used instead of custom WAI-ARIA widgets whenever possible, because of the built-in accessibility features of native HTML widgets. Implementing custom widgets requires greater attention to detail in the coding techniques and patterns, and support for custom widgets may vary, especially for less common widgets.
3. When creating ARIA widgets, pay attention to the semantic structure of the roles. Some roles have required parent or child roles, and some roles have required attributes.
4. When a custom role is assigned to an element, the custom role completely overrides the native role. For example, `<li role=”button”>` will be treated like a button by the accessibility API, not like a list item.
5. The application role should be used sparingly, if at all, because it overrides many assistive technology keystrokes, such as the keystrokes that allow screen reader users to navigate by semantic elements such as headings, landmarks, tables, etc.

### F. Create accessible single-page applications.
Study topics related to single-page applications
1. If the AJAX content is loaded as the direct result of a user action (e.g. activating a button), the screen reader user should be notified that new content has loaded. Methods that can be used to notify screen readers that new content has loaded include:

    a) Sending the focus to the new content

    b) Using aria-live to make an announcement without moving the focus.
2. If the AJAX content is loaded passively (i.e. not as the direct result of a user action like activating a button), users may not need to be notified that the new content has loaded, depending on the importance and urgency of the content and whether the content has been inserted above the user’s current position or not.

### G. Create web content that is compatible with the strategies used by persons with disabilities to access web content.
**Note:** These study tasks are inferred from the Body of Knowledge, not directly stated
1. Differentiate between the strategies and technologies used by people with different kinds of *visual* disabilities

    a) Identify the strategies and technologies used by people who are blind to access web content

    b) Identify the strategies and technologies used by people with low vision to access web content
2. Identify the strategies and technologies used by people with reading difficulties to access web content
3. Identify the strategies and technologies used by people with cognitive disabilities to access web content
4. Identify the strategies and technologies used by people with motor disabilities to access web content
5. Identify the strategies and technologies used by people who are deaf or hard-of-hearing to access web content

## [II. Identify accessibility issues/problems (40%)](II/index.md)
### A. Identify interoperability and compatibility issues.
Study topics related to strategies used by people with disabilities
Some highlights of the types of things to look for include:
1. Keyboard accessibility

    a) Actionable elements (links, buttons, controls, etc.) are focusable with the keyboard

    b) All focusable elements must have a visible focus indicator

    c) Logical tab order

    d) No keyboard trap
2. Touch device accessibility

    a) Sufficiently large touch target size

    b) Allowing different screen orientations

    c) Extra considerations for when the screen reader is turned on 

    d) Custom gesture events must have an alternative method for activation (e.g. by activating a button)

    e) Motion-activated events (e.g. shaking the device) must have an alternative method for activation (e.g. clicking a button)

### B. Determine conformance to accessibility specifications based on accessibility issues found.
Study topics related to determining the level of conformance to accessibility specifications
1. Become familiar with the specifications (WCAG, WAI-ARIA, and ATAG), and know which success criteria apply to which conformance level.
2. Be able to distinguish between failures of accessibility criteria versus other bad accessibility practices that are not referenced in the specifications.

### C. Test with assistive technologies.
Study topics related to testing with assistive technologies
1. Know how to use screen readers to navigate elements such as landmarks, headings, tables, forms, etc.
2. Know how to go forward and backward through focusable content in screen readers (e.g. using the tab key or shift+tab in desktop browsers)
3. Know how to go forward and backward through all content in screen readers (e.g. using the down or up arrow keys in most screen readers).
4. Know the consequences of using contrast enhancement modes such as Windows High Contrast Mode
5. Know how to use the keyboard to navigate forms.
6. Know how to use the keyboard to navigate ARIA custom widgets.
7. Know your own limitations in your assistive technology knowledge. If you’re not experienced, don’t assume something is an error if it may be that you don’t know how to use the assistive technology correctly.
8. Know why it is important to get the opinions and feedback of users with disabilities using their own assistive technologies. 
9. Know which combinations of assistive technologies work best with which browsers. Don’t test on combinations that aren’t recommended or that don’t fully support accessibility.

### D. Test for end-user impact 
Study topics related to testing the end-user impact
1. Understand the value of user testing, with users with a variety of types of disabilities.
2. Think through the consequences of certain types of accessibility flaws. Some times are more damaging than others.
3. Consider the usability of the design, not just the accessibility or just conformance to the specifications.

### E. Use accessibility testing tools effectively.
Study topics related to accessibility testing tools:
1. Know the strengths and limitations of automated testing tools. 
2. Differentiate between the kinds of accessibility issues that can be found with automated tools and issues that require manual testing. 
3. Understand how accessibility software tools can be used at various stages in the web development process (e.g. design/develop/test).
4. Be familiar with the types of software tools available (site-wide scanning, server-based analysis, unit testing, integration testing, browser developer tools, browser add-ons, simulators, guided manual testing, etc.).
5. Know how to generate and translate results into usable analysis, prioritization and categorization, and how to differentiate technical reports from business reports.

## [III. Remediate (fix) accessibility issues (20%)](III/index.md)
### A. Prioritize accessibility issues based on the level of severity.
Study topics related to prioritizing accessibility issues based on the level of severity 
1. **Identify the Issue:** Identify the accessibility issue either in the style, markup, or functionality of the content.
2. **Identify the User Impact:** Associate the issue with the impact on the affected accessibility user. Differentiate between minor issues that can be worked around via advanced accessibility methods and complete blocker issues.
3. **Identify the Legal Risk and Cost Benefit:** Determine whether the issue identified is a legal risk or a potential usability improvement. Take into account factors such as visibility and frequency. Determine the cost benefit provided by the remediation, due to accessibility users’ ability (or current inability) to complete the flow in question.
4. **Determine Level of Effort associated with Issue Remediation:** Differentiate between style, markup, and functionality changes.
5. **Prioritize:** Use the user impact, legal risk, cost benefit, and level of effort to determine severity, identify low-hanging fruit and prioritize all issues.

### B. Recommend strategies and/or techniques for fixing accessibility issues.
Study topics related to recommending strategies and/or techniques for fixing accessibility issues
1. Characterize and differentiate between the ideal/best solution and the “good enough” solution, respecting the particular project, its environment, intended target groups, and resources.
2. Demonstrate the understanding between the fixing of the particular issue and the complete redesign of the web page.
3. Demonstrate the ability to distinguish the feasibility of the particular solution in different contexts.
4. Demonstrate the knowledge of practical and simple hints, leading to better web accessibility.
5.	Communicate the purpose, approach and strategy to remediate.
6.	Ensure that the right stakeholders are aware, educated, and included in implementation recommendations.
7.	Consider the use of maturity models and tools to illustrate progress and sustainability.