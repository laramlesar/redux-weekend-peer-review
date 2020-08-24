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
  - [x] Able to add feedback
    - [x] Data collected on individual pages & components
    - [x] Click on next takes you to the next page in sequence
    - [x] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [x] Thank you page takes you back to the first view
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
    - [x] Reducers are using spread correctly (to keep old data, while adding new)--did not use spread
  - [x] Review Component shows at all times with current redux state
  - [x] React-Redux Working
    - [x] `connect`ing components correctly & dispatching Actions onClick
    - [x] `mapStateToProps` when data is needed from Redux for submission
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
First must be complete for score of _5 - Exceeds Expectations_

- Previous Steps
  - [x] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [x] user can update their score for a step
  - [x] new score is validated to not be empty
  - [x] redux is updated with new score
  - [x] user can continue on to review page and submit as in Base Mode


- Admin View
  - [x] All entries are visible with correct data from inputs
  - [x] Most recent is at the top
  - [x] Can Delete an entry
  - [ ] User is prompted before deleting - no
  - [x] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [x] Styling with Material UI
- [x] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku


## Markdown

```
Hey __iHansy_,

General Feedback.

I would change the numbers to only allow 1-5 even though there is the alert, the background pic is very relaxing and calming 
Very nice 

---
| Functional Requirements | Complete? |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | y |
| Data stored in Redux when navigating from page to page | y |
| User is notified when trying to leave a blank score | y |
| Review Component displays scores and comments from current redux state | y |
| Submit button sends data to the server via Axios | y |
| Confirmaion Page displays after data is POSTed to the server | y |
| Button on Confirmation Page clears Redux and starts a new survey | y |
| Views are broken down into components | y |

---
### Notes:

Notes on the above Functional Requirements.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | y |
| Commits are descriptive of the changes made or feature added | y |
| Readme file updated | y |
| Appropriate amount of code comments | y |
| Code is consistently formatted |y |
| Server code organized with router & module files | y |

---
### Notes:

Notes on General Items

```
