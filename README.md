# Francis' Web Dev Course
### Setup
- Install [npm](https://www.npmjs.com/):

```bash
brew install node@12
```
- Verify you installed it correctly:

```bash
which npx # will output something like /usr/local/opt/node@12/bin/npx
```

- Create a dedicated workspace for this stuff:

```bash
cd
mkdir -p ws
```

- Bootstrap a project:
```bash
npx npx create-react-app deanna-hello-world # This will take a while...
```

- [Create a new empty github repo](https://github.com/new)
  - Call it "deanna-hello-world" for consistency

```
REPO="<Repo URL of what you just made i.e. https://github.com/francisphan/foobar.git>"
cd ~/ws/deanna-hello-world
git remote add origin https://github.com/francisphan/foobar.git
git push -u origin master
echo "Go back to $(echo $REPO | sed 's/.git$//g') to make sure that you did it right"
```
- Your github repo should display all the bootstrapped code
- The provided `README` will tell you how to create a local webserver.

## Assignment 1
- Create a button that when _clicked_ toggles a display
  - **Acceptance Criteria**:
    - If not displayed -> clicking button should display it
    - If it is displayed -> clicking button will hide it
    - Button is in the middle of the page


```
Hello World!
```

## Assignment 2:
- Write unit tests for assignment 1
  - **Acceptance Criteria**:
    - Utilize [jest](https://jestjs.io/) and [enzyme](https://enzymejs.github.io/enzyme/)
    - Unit test that will show when button clicked, expected state changes happen

## Assignment 3:
- Utilize [react-redux](https://redux.js.org/) to manage app state. 
- **DO NOT** use React Redux Hooks or any React Hooks yet (this'll be a future assignment since this is relatively "new" tech, so it's good to know both ways)
  - **Acceptance Criteria**:
    - Text display state is managed via [redux](https://redux.js.org/)
    - Unit tests modified accordingly

### Additional readings (in no particular order)
- [npm](https://www.npmjs.com/): "Node Package Manager" a registry that people publish JS code/libraries to for you to use.
- [webpack](https://webpack.js.org/): Serves your HTML, CSS, JavaScript to your browser
- [React](https://reactjs.org/): A JavaScript framework - also probably the most widely known/asked for 
- [jest](https://jestjs.io/): JavaScript testing framework
- [enzyme](https://enzymejs.github.io/enzyme/): JavaSript Testing Utility library that makes it easy to test React components
- [react-redux](https://redux.js.org/): Javascript library to manage and maintain application state store
