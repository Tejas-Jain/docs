## Select Screen Use Case

### Use Case ID
UC001

---
### Description
Allow user to prompt and select the screen from the given tab, window or desktop screens.

---
### Actors
- **Actor 1**: User of the extension

---
### Preconditions
- None

---
### Trigger
- User Select the screen select button.
- User click the capture button.
---
### Main Flow
1. User click the screen select button.
2. User select the screen from the given tabs, windows, or screens.
3. User confirms its selection by clicking **OK button** .
4. User captures and process the screenshots.
5. User terminate the session by clicking the select screen button again.
---
### Alternative Flows
- User initiates screen selection by clicking capture button if no screen is selected.
- User Terminates screen monitoring by clicking stop sharing button on the screen-sharing notification window.
---
### Postconditions
- User has successfully selected the screen.
- The window shows screen is sharing notification window.
---
### Exception Flows
- User click the cancel button before or after selecting the screen. This is shown by console log "Permission not granted".
---
### Special Requirements
- Screen has screen sharing rights.
---
### Assumptions
- User don't want to capture any personal or sensitive information, as the screenshots are processed by third party libraries.
---
### Author
- Tejas Jain
---
<br><br>
---
---

## Capture Screen Use Case

### Use Case ID
UC002

---
### Description
Allows user to capture the selected screen along with the text box content.

---
### Actors
- **Actor 1**: User of the extension

---
### Preconditions
- Screen Sharing has already started.

---
### Trigger
- User the screen capture button [Button 2].
- User click the picture in picture mode [pause button].
---
### Main Flow
1. User has a selected screen.
2. User triggers the screen capture.
3. Screen got captured and reflected in the bottom panel.

---
### Alternative Flows
- User click red cross button on small panel to remove captured notes.
---
### Postconditions
- The captured screen is reflected in the bottom panel.
---
### Exception Flows
- None
---
### Special Requirements
- Screen sharing is already started.
---
### Assumptions
- User don't want to capture any personal or sensitive information, as the screenshots are processed by third party libraries.
---
### Author
- Tejas Jain
---
<br><br>
---
---

## Go Picture in Picture Mode

### Use Case ID
UC003

---
### Description
Allows user to go in picture and picture mode and allow multitasking.

---
### Actors
- **Actor 1**: User of the extension

---
### Preconditions
- Screen sharing has already started.

---
### Trigger
- User the Picture in Picture Button to enter PiP mode [Button 3].
- User clicks the PIP mode again to exit the pip mode.
---
### Main Flow
1. User has a selected screen.
2. Clicks the Pip Mode Button.
3. A small window appears on the bottom right corner of the screen aka PiP window.
4. The current selected screen is visible in the PiP window.

---
### Alternative Flows
- User click the PiP mode button again to exit.
---
### Postconditions
- A small screen showing the current selected screen is visible.
---
### Exception Flows
- No screen is shared for monitoring results in alert of "First please select the screen using First button".
---
### Special Requirements
- None
---
### Assumptions
- User selected screen is visible to on any window the user will go to.
---
### Author
- Tejas Jain
---
<br><br>
---
---

## Text Box Use Case

### Use Case ID
UC004

---
### Description
Allows user to add additional text notes with the captured screens.

---
### Actors
- **Actor 1**: User of the extension.

---
### Preconditions
- The user has selected some screen for saving the associate the current written note with.

---
### Trigger
- User types in text note in the text box.

---
### Main Flow
1. User has a selected screen.
2. User has typed in some additional notes for the screen he is about to capture.
3. User triggers the screen capture.
4. Screen got captured and reflected in the bottom panel, without the text note which will be visible only in the final downloaded PDF.

---
### Alternative Flows
- User clears the textbox and no text will be saved with the screenshot.

---
### Postconditions
- The captured screen is reflected in the bottom panel and the textbox got cleared automatically.
---

### Exception Flows
- If no screen is selected and captured is clicked after writing the notes, a screen select prompt will appear.
---

### Special Requirements
- None
---

### Assumptions
- If user text exceeds 200 words, it will be wrapped to new blank page without any screenshot.
---

### Author
- Tejas Jain
---
<br><br>
---
---


## Download PDF Use Case.

### Use Case ID
UC005

---
### Description
Allows user to download all data captured till now.

---
### Actors
- **Actor 1**: User of the extension.

---
### Preconditions
- The system should have atleast 1 captured screen and the bottom panel containing the screen is not empty.

---
### Trigger
- User click download PDF.

---
### Main Flow
1. User has a selected screen.
2. User has typed in some additional notes for the screen he is about to capture.[Optional]
3. User triggers the screen capture.
4. Screen got captured and reflected in the bottom panel, without the text note which will be visible only in the final downloaded PDF.
5. User click Save PDF button.

---
### Alternative Flows
- User leaves the window without saving the captured screenshots.

---
### Postconditions
- A PDF file is downloaded without 5-10 seconds(depending on computer processing power) of clicking the button.
---

### Exception Flows
- If no screenshot is present to be saved, no pdf file is downloaded.
- If number of screenshots exceeds 100, a blank page file will be downloaded.
---


### Author
- Tejas Jain
---
<br><br>
---
---
