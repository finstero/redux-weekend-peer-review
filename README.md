# Weekend Challenge 11 - React-Redux Feedback Form
Mary
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
  - [x] Able to add feedback
    - [x] Data collected on individual pages & components
    - [x] Click on next takes you to the next page in sequence
    - [x] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [submit takes you back, no thank you] Thank you page takes you back to the first view
    - [x] Old Data is cleared on form completion

- Client code:
  - [x]  Individual components for each form part
  - [x]  Redux setup complete
    - [x] Store linked to react with `<Provider>`
    - [x] Store setup with reducer(s) and logger middleware 
  - [x] Reducers & Actions Working
    - [x] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [x] Actions have a `type` key, and `payload` if sending data
    - [x] Reducers are returning a new state, or the old state (not mutating)
    - [x] Reducers are using spread correctly (to keep old data, while adding new)
  - [x] Review Component shows at all times with current redux state
  - [x] React-Redux Working
    - [x] Dispatching actions onClick
    - [x] Grabbing data from the redux store with `useSelector`
  - [x] Axios POST request to add feedback


- Server code:   
  - [x] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [x] Multiple git commits showing incremental progress
  - [x] Commits are descriptive of the changes made or feature added 
  - [x] Has .gitignore with node_modules
  - [x] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [x] Appropriate amount of code comments
  - [x] Code is consistently formatted
- Client
  - [x] Appropriate use of HTML tags
  - [x] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of  _Exceeds Expectations_

- Previous Steps
  - [ ] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [ ] user can upate their score for a step
    - [ ] new score is validated to not be empty
    - [ ] redux is updated with new score
  - [ ] user can continue on to review page and submit as in Base Mode


- Admin View
  - [x] All entries are visible with correct data from inputs
    - [ ] Most recent is at the top
  - [x] Can Delete an entry
    - [x] User is prompted before deleting
  - [? not sure what componentDidMount is] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [x] Styling with Material UI
- [x] Ability to flag a feedback item on `/admin` for further review
- [not sure] Deployed to Heroku


## Markdown

```
Hey Mary,

Awesome job!

General Feedback.

---
| Functional Requirements | Complete? yes |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | yes |
| Data stored in Redux when navigating from page to page | yes |
| User is notified when trying to leave a blank score | no, but submit button won't work if no star is selected |
| Review Component displays scores and comments from current redux state | yes |
| Submit button sends data to the server via Axios | yes |
| Confirmaion Page displays after data is POSTed to the server | no |
| Button on Confirmation Page clears Redux and starts a new survey | no confirmation page, but on submit you go back to survey start. |
| Views are broken down into components | yes |

---
### Notes:

Notes on the above Functional Requirements.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | yes, 61 |
| Commits are descriptive of the changes made or feature added | yes |
| Readme file updated | yes |
| Appropriate amount of code comments | yes |
| Code is consistently formatted | yes |
| Server code organized with router & module files | yes |

---
### Notes:

Looks great! Graph in admin is super cool.
Notes on General Items

```
