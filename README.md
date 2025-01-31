# PetJournal
Log a recollection of memories from your Pet's life. 

<img src="https://img.shields.io/badge/JavaScript-323330?logo=javascript&logoColor=F7DF1E" />
<img src="https://img.shields.io/badge/MongoDB-4EA94B?logo=mongodb&logoColor=white" />
<img src="https://img.shields.io/badge/Express.js-000000?logo=express&logoColor=white" />
<img src="https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB" />
<img src="https://img.shields.io/badge/Node.js-43853D?logo=node.js&logoColor=white" />
<img src="https://img.shields.io/badge/Redux-593D88?logo=redux&logoColor=white" />
<img src="https://img.shields.io/badge/Material--UI-0081CB?logo=material-ui&logoColor=white" />
<img src="https://img.shields.io/badge/Heroku-430098?logo=heroku&logoColor=white" />
<img src="https://img.shields.io/badge/Netlify-00C7B7?logo=netlify&logoColor=white" />

<details><summary>Requirements</summary>

- [x] A Backend
- [x] A Frontend
- [x] CRUD
- [x] Authentication
- [x] Local Storage
- [x] Include Wireframes
- [x] Clean JSX (html)
- [x] Clean CSS (Material UI makeStyles)
- [x] Hosted Backend (Heroku)
- [ ] Hosted Frontend (Netlify)
- [x] Pushed to Github
- [x] Readme file 
</details>

<details><summary>Wireframes</summary>

![Landing Page](/assets/Landing%20Page.png)
![Login](/assets/Login.png)
</details>

<details><summary>What does the project answer?</summary>

* Folder structure - from many source codes I've seen before I see so many folders that I haven't seen in react. I wanted to expand where possible to understand large folder structures. 
* Redux - 1. New Job uses it. 2. State management as I struggled with understanding the hierarchy of react state and having just one global Redux Store simplifies it greatly. 
* Everyone loves pets.
</details>

<details><summary>Learned along the way</summary>

* dotenv files for secure credentials
* MondoDB Atlas and Compass are both the same for viewing db data. 
* router.get('/', (req,res)) vs router.route("/").get((req, res)
* You have to use CORS before you specify routes. 
* app.use("/") has to be last otherwise it'll be the default. Can't access "/memory"
* Todo tree from the marketplace
* The precision of capitalisation of db fields. Couple hours of frustration there.
* That I don't really care for Bootstrap / react-bootstrap's jsx implementation.
* JSX Fragments as a parent to use multiple .
* Redux is easier to understand and use with React Hooks now a thing. But that doesn't make it easy to understand. 
* Redux creates a lot more files and folders but that's a small price when trying to understand state. 
* A thunk is a function that wraps an expression to delay its evaluation. (allows async await)
* Redux Workflow: First we fill in the form, once filled in, we dispatch an action (signin) passing the formData and History, the action calls the post request api for some { data }, then dispatch an AUTH action.
* Action creators create objects → objects are dispatched to the store → the store invokes reducers → reducers generate new state → listeners are notified of state updates.
* Creating CONSTANTS for strings as strings don't trigger error logs. ie Actions and reducers.
* Dynamic Titles with ternary operators inside JSX: {currentId ? "Edit" : "Create"} a Memory
* Using ternary operators to create 2 components in 1 field. 
* Optional Chaining with ?. operator.
* Using the Chrome Application tab to monitor Local Storage Token
</details>

<details><summary>Understanding Folder Structure</summary>

* assets: for images etc
* components: for react components. 
* api: contains axios middleware. 
* actions: contain an action type and a payload(data from a function to be used to update state)
* reducers: implement the Action
* styles.js files: For MaterialUI's { makeStyles } theming. 
* constants - used to eliminate any "strings" being hardcoded. 
* Auth: contains everything for the authentication form
* Procfile: required for Heroku
</details>

<details><summary>Feature Requests</summary>

* Landing Page. 
* SweetAlerts2 (at first, and then custom)
* Google OAuth
* React Masonry CSS (for tumblr styled layout instead of grid)
* Filter: Show only user created memories. 
* Add a list of Pets per user. When creating a memory select Pet to add. 
* Filter: Show only created memories of Pet
* Each Pet added to memory has a Pet avatar with link to Pet bio. 
* Like functionality for memories. 
* Search
* Search on Pets
* Search on Tags
* Backend Testing. 
* Frontend Testing. 
* Custom upload image button. Add label for component rather than an input.
</details>

<details><summary>Bugs</summary>
Memory date stamp isn't consistent with date created. 
Password visibility is different between signin and signup. 
autofill active even though autoComplete="off"
When changing to sign in mode email isn't focused {!isSignup && autoFocus}. tried, failed. 
Tabbing through the signup form focuses on the visibility icon. 

</details>

<details><summary>Installation</summary>

## Server: 
Node:
npm install
npm start

## Client:
npm install 
npm audit fix --force
npm start

## Heroku: 
heroku logs --tail

</details>

<details><summary>Presentation</summary>

## What to show: 
### Landing page
 - just the posts, no interaction. 
### Sign In
- Sign Up action is displayed from JSX if logic. 
- Can't edit something that's not that users. 
### Create Memory
- create memory
- name is automatically populated
- tagging via mapping and splitting
- date format from 'date-fns' instead of momentJs. 
- Edit / delete . 
### Logout
- logout takes you back to signin. 
- paw takes you home.

## How long did this take? 
From VS Code Extension "Code Time"
### A Pet's Life: 
Code time : 22.2 hrs
Keystrokes : 17,212
### PetJournal (the original project name):
Code time : 9.6 hrs
Keystrokes : 9,454
### ClockInClockOut (the first project): 
Code time : 14.9 hrs
Keystrokes : 14,009

### End Result: 
46.7 Hours (A week of 9hour days) to make a project that would now only take about 3hours. 

### Am I proud of it? 
... not in it's current state. 
But I will be working on it to make it into something quite nice.  

## What next? 
### Start from scratch with:
- React Native
- Mobile First
- TDD
- React Context instead of Redux.

</details>