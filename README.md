
## Hello everyone and welcome to React!

Below are some helpful resources that will help you in this module

1. If you're using Atom as your text editor, download the [JSX plugin](https://orktes.github.io/atom-react/). This will give you some pretty great JSX syntax highlighting and will make coding in React much easier. After the package is installed, open up your `preferences` in Atom. Navigate to `packages` search for `react` then click `settings` amd make sure you check the box next to `Enabled For All JavaScript Files`

2. Install the [React Devtools Chrome Extension](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en). This gives you access to some pretty great tools that make it a lot easier to debug your programs in React. Here is the [repo](https://github.com/facebook/react-devtools#faq) for the extension.

3. Please take some time to read [Thinking in React](https://reactjs.org/docs/thinking-in-react.html), a short article straight from the official React documentation that walks through thinking about your React applications and component structure.

4. Most importantly, the official [React Documentation](https://reactjs.org/), courtesty of Facebook. THX Facebook for creating this stellar library.

5. As a bonus, take a look at [error handling in fetch](https://gist.github.com/odewahn/5a5eeb23279eed6a80d7798fdb47fe91)

```
fetch("/api/foo")
  .then( response => {
    if (!response.ok) { throw response }
    return response.json()  //we only get here if there is no error
  })
  .then( json => {
    this.props.dispatch(doSomethingWithResult(json)) 
  })
  .catch( err => {
    err.text().then( errorMessage => {
      this.props.dispatch(displayTheError(errorMessage))
    })
  })
  ```


![Zuckerberg](https://media.giphy.com/media/MeMue8HRo4Hsc/giphy.gif)


<p class='util--hide'>View <a href='https://learn.co/lessons/some-useful-tools-for-writing-react'>Some Useful Tools for Writing React</a> on Learn.co and start learning to code for free.</p>
