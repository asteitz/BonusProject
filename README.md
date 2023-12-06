# Bonus Project - Reminder App
<span style="font-size: smaller;"><strong>Ashley Steitz and Jacob Fritz worked on this as partners</strong></span>

---
<span style="font-size: smaller;"><strong> Description </strong> </span>
In our efforts to complete the Bonus project we implemented an interactive Ui (User Interface) that allows the user to create a reminder and select a date and time.

This app allows for a user to:
- Create a reminder
- Add a description
- Select a date and time
- Delete the reminder

To begin we integrated SQL into our data handling to store our user entries. We used a recycler view to store the reminders and display them on the main reminder page (screen)
and it allows for users to scroll and view all reminders without fear of losing the content when it goes off the page!
<br>
<br>
The app opens and has a + sign at the top for the user to create a reminder in the ribbon. When
pressedm they are navigated to the next fragment, which prompts them to add a title, description,
and then selecte a date for the reminder as well as a time.
<br>
After the user enters all fields, then they can press the escape button which takes them to the main screen and they can delete or add notes as they please
<br>
<br>
On the main screen after the trashcan icon is selected (this is a delete button) the user is greeted by a dialog that prompts
them to select "YES" or "NO", confirming or denying their selection to delete their note. If they delete the note the note title and body are deleted from the data base. If "NO" is selected,
then nothing happens to the database.



## Functionality
'*' indicates tested in GIF  
The following **required** functionality is completed:
<br>
Safeargs and View Groups were implemented to transfer data from MainActivity.kt to Fragment1.kt. This allows us to gather the user data and translate it in real time!

**Demonstrated**
<br>
**START**
<br>
* [ + ] -> [TITLE:Feed Dog] [Description:feed dogs when you get home] [Date: Dec. 8] [Time: 7:30] [esc]
* [ + ] -> [TITLE:Feed Cat] [Description:feed cat when you get home] [Date: Dec. 9] [Time: 17:30] [esc]
* [ + ] -> [TITLE:Submit Final project] [Description:submit C323 final project] [Date: Dec. 13] [Time: 11:59] [esc]
* [Feed Dog] [trashcan] [yes]
* [Feed Dog] [trashcan] [no]

<br>

**END**


---
## Video Walkthrough
Watch a demonstration of the different options when working with the notes app in the gif available on Github
Here's a walkthrough of a few translations:
**there was a slight adjustment to the buttons size that was implemented after the video was created and the changes do not alter the performance of the app -> however this changes clossly
reflects the UI requested in the PDF**
<br>
<img src='https://github.com/asteitz/Project_6/blob/master/app/src/main/java/com/example/project6/RecordingNotesApp.gif' title='Project6 Video Walkthrough' width='50%' height = '50%' alt='Video Walkthrough' />

GIF created with [CloudConvert](https://cloudconvert.com/).

## Notes
UI Challenges:
- Had the wrong auto set for the view of the remidners (needed to be wrap contents instead of match parent)
    - due to this we were not able to see the reminders they popped up
- Integrating a recycler View into the UI for the main notes page
- Adding in a constraint layout to keep the buttons in place when the user is typing
- Adding function calls inside the xml files

Backend Challenges:
- Big issues with having the data being passed between the fragment and the database had to request extension and attend office hours
- Difficult time with the gradle files and versions not being compatible
- Struggled integrating the SQL database into the calls when a button is pressed
- Working with an adapter to communicate between the view model and the database

## License

    Copyright [2023] [Ashley Steitz, Jacob Fritz]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
