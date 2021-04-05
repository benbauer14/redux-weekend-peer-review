# Weekend Challenge 11 - React-Redux Feedback Form

## Instructions

Reviewing code is an important role developers play. We're going to practice reviewing code from others.

- Get the repo url from your partner
- Get your partner's project running on your computer
- Review the code from your partner and give relevant feedback
- Complete the Markdown section and submit that in the notes section on the assignment app. (Make sure you include who's code you reviewed.)

Practicing compassionate code reviews is important (you can learn more from this video on the topic: https://www.youtube.com/watch?v=Ea8EiIPZvh0 )

## Review Checklist

## Base Required Features 

- Multi-Part Form:  
  - [ ] Able to add feedback
    - [ ] Data collected on individual pages & components
    - [ ] Click on next takes you to the next page in sequence
    - [ ] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [ ] Thank you page takes you back to the first view
    - [ ] Old Data is cleared on form completion

- Client code:
  - [ ]  Individual components for each form part
  - [ ]  Redux setup complete
    - [ ] Store linked to react with `<Provider>`
    - [ ] Store setup with reducer(s) and logger middleware 
  - [ ] Reducers & Actions Working
    - [ ] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [ ] Actions have a `type` key, and `payload` if sending data
    - [ ] Reducers are returning a new state, or the old state (not mutating)
    - [ ] Reducers are using spread correctly (to keep old data, while adding new)
  - [ ] Review Component shows at all times with current redux state
  - [ ] React-Redux Working
    - [ ] Dispatching actions onClick
    - [ ] Grabbing data from the redux store with `useSelector`
  - [ ] Axios POST request to add feedback


- Server code:   
  - [ ] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [ ] Multiple git commits showing incremental progress
  - [ ] Commits are descriptive of the changes made or feature added 
  - [ ] Has .gitignore with node_modules
  - [ ] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [ ] Appropriate amount of code comments
  - [ ] Code is consistently formatted
- Client
  - [ ] Appropriate use of HTML tags
  - [ ] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of _5 - Exceeds Expectations_

- Previous Steps
  - [ ] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [ ] user can upate their score for a step
    - [ ] new score is validated to not be empty
    - [ ] redux is updated with new score
  - [ ] user can continue on to review page and submit as in Base Mode


- Admin View
  - [ ] All entries are visible with correct data from inputs
    - [ ] Most recent is at the top
  - [ ] Can Delete an entry
    - [ ] User is prompted before deleting
  - [ ] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [ ] Styling with Material UI
- [ ] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku


## Markdown

```
Hey ...,

General Feedback.

---
| Functional Requirements | Complete? | Y
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | yes |
| Data stored in Redux when navigating from page to page | yes |
| User is notified when trying to leave a blank score | yes? – user cannot proceed but no alert |
| Review Component displays scores and comments from current redux state | yes |
| Submit button sends data to the server via Axios | yes |
| Confirmaion Page displays after data is POSTed to the server | yes |
| Button on Confirmation Page clears Redux and starts a new survey | no – returns to homepage but does not appear to reset redux to initial state |
| Views are broken down into components | yes |

---
### Notes:
Overall good functionality. I could enter any value that I wanted for the ratings so I gave a 10 rating on how I was feeling. Also, an alert may be a good warning that the user can’t proceed but the user was unable to move forward. The redux was not reset after returning home. All in all, the basic functionality was good and worked as described.

Notes on the above Functional Requirements.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | yes - 22 |
| Commits are descriptive of the changes made or feature added | yes |
| Readme file updated | no |
| Appropriate amount of code comments | no – very few comments throughout app |
| Code is consistently formatted | yes |
| Server code organized with router & module files | yes |

---
### Notes:

Notes on General Items
Good number of commits that were well described. Readme file needs updating especially if it is a public repo. Also, more comments would be good for anyone less familiar with the code. Great formatting and easy to follow routes. Code is clean and easy to follow.
![image](https://user-images.githubusercontent.com/76824772/113595506-b96b9780-95fe-11eb-999b-2bfcb55a364f.png)

