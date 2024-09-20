# M5.2 Lab 

## Overview
This projects excercises current accessibility practices for disabled and impaired users. 

## Runing
#### 1. Navigate to the Folder
Navigate to the folder where you want to save the repository by typing:

```bash
cd path_to_your_directory
```
#### 2. Clone the Repository

Clone the repository using the following command:

```bash

git clone https://github.com/username/repository-name.git
```
(Replace username and repository-name with the actual GitHub username and repository name.)

#### 3. Navigate to the Repository Directory

Navigate to the repository directory:

```bash

cd repository-name
```
#### 4. Open the HTML File in Your Browser

In your terminal or file explorer, navigate to the directory where the HTML file is located.

    Find the .html file you want to view.
    Double-click on the HTML file, or right-click and choose Open with and select your preferred web browser (e.g., Chrome, Firefox, etc.).

Your HTML file should now open in your browser.

## Accessibility Lab Answers

### Color
- The text is difficult to read because of the current color scheme. Can you do a test of the current color contrast (text/background), report the results of the test, and then fix it by changing the assigned colors?

The test results came back as the text is impossible to read for some users so I changed the background color from green to white.

### Semantic HTML
- The content is still not very accessible — report on what happens when you try to navigate it using a keyboard.
    When you try to navigate with the keyboard some elements are not focused and are inaccessible. 
- Can you update the article text to make it easier for screen reader users to navigate?
    Surrounded text with p tags so that screen reader users can navigate.
- The navigation menu part of the site (currently wrapped in `<div class="nav"></div>`) could be made more accessible by putting it in a proper HTML semantic element. Which one should it be updated to? Make the update.
    The proper html tag would be nav for a navigation bar.

### Image Accessibility
- The images are currently inaccessible to screen reader users. Can you fix this?
    we can use the alt tag and give a description of the image for screen reader users.

### The Audio Player
- The `<audio>` player isn't accessible to hearing-impaired (deaf) people — can you add some kind of accessible alternative for these users?
    We can add a audio transcript for deaf users. 
- The `<audio>` player isn't accessible to those using older browsers that don't support HTML audio. How can you allow them to still access the audio?
    If the browser doesn't support audio HTML then we can have a download link to the audio.

### The Forms
- The `<input>` element in the search form at the top could do with a label, but we don't want to add a visible text label that would potentially spoil the design and isn't really needed by sighted users. How can you add a label that is only accessible to screen readers?
    we can use the aria-label tag to be accessed by screen readers.
- The two `<input>` elements in the comment form have visible text labels, but they are not unambiguously associated with their labels — how do you achieve this? Note that you'll need to update some of the CSS rules as well.
    For each input element we can add a name abd a comment label.

### The Show/Hide Comment Control
- The show/hide comment control button is not currently keyboard-accessible. Can you make it keyboard-accessible, both in terms of focusing it using the tab key and activating it using the return key? 
    Yes, by using the tabindex tag and modifying the current js code to work with the return key.

### The Table
- The data table is not currently very accessible — it is hard for screen reader users to associate data rows and columns together, and the table also has no kind of summary to make it clear what it shows. Can you add some features to your HTML to fix this problem?
    By using the scope tag such as every row and column can be identified by a screen reader and we 
    can a table description to tell the user what the data shows.

### Other Considerations
- Can you list two more ideas for improvements that would make the website more accessible?
    Two things to make the site more accessible is to increase the font size of the text because it is 
    too small, as well as having more contrast between the colors to easily differentiate elements.

## Sources and Credits

- ARIA practices: https://www.w3.org/WAI/ARIA/apg/practices/
- table: https://www.w3schools.com/tags/att_scope.asp
- Action Listener: https://www.w3schools.com/js/js_htmldom_eventlistener.asp
- Labels: https://www.w3schools.com/tags/tag_label.asp
- Descriptions: https://chatgpt.com
