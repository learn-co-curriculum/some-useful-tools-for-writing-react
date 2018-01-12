
## Hello everyone and welcome to React!

Below are some helpful resources that will help you in this module

1. If you're using Atom as your text editor, download the [JSX plugin](https://orktes.github.io/atom-react/). This will give you some pretty great JSX syntax highlighting and will make coding in React much easier. After the package is installed, open up your `preferences` in Atom. Navigate to `packages` search for `react` then click `settings` amd make sure you check the box next to `Enabled For All JavaScript Files`

2. [prettier-atom](https://github.com/prettier/prettier-atom) is another great plugin. It's *very* opinionated but will automatically format you JS and React when you save a file. Use it if you want to and enable/disable semicolons depending on your preferences.

3. You might also want to enable [autosave](https://atom.io/packages/autosave) in Atom. This will automatically save your files onBlur or when they're closed. Open up `preferences/packages` in Atom then search for autosave, open `settings` and enable it if you want.

4. Please remember that the [setState](https://reactjs.org/docs/react-component.html#setstate) method in React is [asynchronous](https://medium.com/@wereHamster/beware-react-setstate-is-asynchronous-ce87ef1a9cf3).

5. You've likely seen or will see the warning that `each child in an array or iterator should have a unique key prop`.
Example: 
```
this.state.hogs.map((hog, index) => (
  {/*AVOID THIS*/}
  <HogTile key={index} />
  {/*Do this instead*/}
  <HogTile key={hog.id} />
))
```
Essentially, React is telling you that any child components should have a unique identifier or [key prop](https://reactjs.org/docs/lists-and-keys.html#keys).  When passing your components key props, avoid using the index while you're iterating as a key as it is an [anti-pattern](https://medium.com/@robinpokorny/index-as-a-key-is-an-anti-pattern-e0349aece318).

6. You may also want to be cautious of [setting the initial state of a component based on props](https://medium.com/@justintulk/react-anti-patterns-props-in-initial-state-28687846cc2e).
```
class Hog extends React.Component {
  constructor(props) {
    super(props)
    this.state = {
    //try to avoid this as it violates single source of truth
      hogs: props.hogs
    }
  }
}
```


7. [Semantic UI for React](https://react.semantic-ui.com/introduction) is a great CSS library written specifically for React. Make sure you read the [usage](https://react.semantic-ui.com/usage) section of the docs to see how to incorporate it into your React projects. **Make sure you're reading the docs for the react version of semantic, not the vanilla JS one.** Their other library uses jQuery which does not play well with React at all.

8. Install the [React Devtools Chrome Extension](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en). This gives you access to some pretty great tools that make it a lot easier to debug your programs in React. Here is the [repo](https://github.com/facebook/react-devtools#faq) for the extension.

9. Please take some time to read [Thinking in React](https://reactjs.org/docs/thinking-in-react.html), a short article straight from the official React documentation that walks through thinking about your React applications and component structure.

10. Most importantly, the official [React Documentation](https://reactjs.org/), courtesty of Facebook. THX Facebook for creating this stellar library.


![Zuckerberg](https://media.giphy.com/media/MeMue8HRo4Hsc/giphy.gif)


<p class='util--hide'>View <a href='https://learn.co/lessons/some-useful-tools-for-writing-react'>Some Useful Tools for Writing React</a> on Learn.co and start learning to code for free.</p>
