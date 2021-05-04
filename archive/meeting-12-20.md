# Hi Team Hack,

Hope you are doing well!  I hope everyone had a great Thanksgiving and Cyber Deal Weekend.  Happy Holidays as we move into the last month of 2020.  Now it's time to meet up again!

We will be having our third meetup on Wednesday at 6pm PST via ZOOM. 

`>>` [RSVP Here for ZOOM LINK](https://zoom.us/meeting/register/tJEkc-qvqD8pH9UDSsN71RevbqFeVhGp8xYr) ❄❄❄

>> You will need a Zoom account to join the meeting (free), as we require everyone to sign in for security and safety issues.

### 👋 Agenda

We will be meeting up to talk through the __React StoryBook__ project we are working on.  As we get into December, my hope is that we can have more components built out and added to a staging server so we can show off our work to the world.

I would like to also start trying out some Github Actions for CI/CD so we can see our work on a staging server.  The way I envision this would be pull requests could be submitted, then auto unit-tested and if successful, deployed to a staging server (possibly integrated with Github/Azure or some other environment).  If anyone wants to help with setting this up, please let me know.

### 🤔 What You Should Do

__Continue to write code__ for your component.  

If you haven't chosen a component to build yet, now is the time to get actively involved.  You can start off by reviewing issues on the [React Storybook Project Board](https://github.com/team-hack/react-components/projects/1).  If you want to work on something custom, feel free to create your own component and start an issue.

For those of you already working on components, here is a recommended file and folder structure:

```shell
src/
  components/
      MyComponent/
        tests/
          MyComponent.test.js | .tsx
        MyComponent.js | .tsx
        MyComponent.stories.js | .tsx
        MyComponent.css
        MyComponent.stories.mdx (optional) 
        index.js | .tsx
```
You don't have to use TypeScript currently, but it's a good idea to implement it into practice -- as the React and Angular communities are beginning to use TypeScript more often with their own code.  

The __focus__ of this project is good User Interface.  So beyond working with tooling and learning things like TypeScript, I care that the components are __reusable__, __aesthetically appealing__ and __useful__.  Key areas to really work are in your Component, Stories and CSS files.  

For example, if you create an `Alert`, think about how someone else might use your `Alert` Component and what are all the cool options (props) you can give them?  Does your component support any event handlers (e.g. onClick, onFocus, onBlur)?  Does your component support Accessibility?  Is your component Unit Tested (see below for more discussion).

### ⭐ Keep Up To Date

I hope by now, you are all familiar with how to __make feature branches and add pull requests__ to the main repo.  You should also be sure to keep your development in sync with the upstream repo often, to avoid any potential merge conflicts -- especially with common files like `package.json` and `tsconfig.json` as some work has been done there.

To keep in sync, simply:

```shell
git fetch upstream
git merge upstream/main 
```

Be sure that you merge to your local `main` branch and not your local development feature branch, aka `<some other branch name>` -- as any changes you pull from upstream may destroy your development work.  When you are sure you are good to go with your development feature branch, you can repeat the same process to your dev branch:

```shell
git fetch upstream
git merge upstream/<my branch>
```

As always, push up your __feature__ branch to your own forked repo, then make a pull request to the [Team Hack](https://github.com/team-hack) repo.  If the changes look good, we will merge them to the `main` branch.  If the changes have issues, we will close the issue and send the PR back to you with suggestions for fixing.  You will need to open another PR if your issue is closed.

### 🧪 Create Some Unit Tests

To get the CI/CD server going, we need to make sure over time we begin writing Unit Tests for our components.  This will be a point of discussion at our meeting; as well as something documented via our Issues.  

Out of the box, our React Storybook supports Jest, and [there are tutorials for using Jest on the Storybook Tutorial webpage](https://www.learnstorybook.com/intro-to-storybook/react/en/get-started/).  To write a test, in your project folder, create a `tests` folder, then add `MyComponent.test.js | tsx` inside for Jest to automatically include.   Write your tests inside the test file, some ideas for tests include:

- Component appears on the Storybook
- Other components with variant props appear on Storybook
- Does something onClick, onFocus

Run `yarn test --watchAll` from a second command shell and see your tests run in action.  

### 💬 Chat On Discord (or Github Issues)

I know a lot of you are still learning and trying to catch up.  If you are getting stuck, feel free to reach out to me or anyone on Discord and we can try to help you out via some Paired Programming (Zoom session or Google Meets).  It's so easy to share a screen and work together in this age -- a decade ago when I started learning, I had to drive out to coffee shops and meet people -- now all that is instant for you.   Take advantage of accelerated learning!

### 🚂 See you Wednesday at 6PM!

`>>` [RSVP Here for ZOOM LINK](https://zoom.us/meeting/register/tJEkc-qvqD8pH9UDSsN71RevbqFeVhGp8xYr)
