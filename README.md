## Hello everyone and welcome to React!

Below are some helpful resources that may accelerate your React learning:

1. If you're using Atom as your text editor, download a JSX plugin (a quick search for 'JSX' will reveal the most popular ones). This will give you some pretty great syntax highlighting for code that is specific to React, and will make coding easier. After the package is installed, open up your `preferences` in Atom. Depending on which package you choose, you may have to edit its settings so that it is the default syntax highlighter for files appended with `.jsx`

2. Install the [React Devtools Chrome Extension](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en). This gives you access to some pretty great tools that make it a lot easier to debug your programs in React. Here is the [repo](https://github.com/facebook/react-devtools#faq) for the extension.

3. Most importantly, the official [React Documentation](https://reactjs.org/), courtesy of Facebook. While you won't have the time to read over all of it now, it might be good to have bookmarked while you learn React.

4. As a bonus, take a look at [error handling in fetch](https://gist.github.com/odewahn/5a5eeb23279eed6a80d7798fdb47fe91)

```
fetch("/api/foo")
  .then(response => {
    if (!response.ok) { throw response }
    return response.json()  //we only get here if there is no error
  })
  .then(json => {
    doSomethingWithResult(json)
  })
  .catch(err => {
    err.text().then(errorMessage => {
      displayTheError(errorMessage)
    })
  })
```

<p class='util--hide'>View <a href='https://learn.co/lessons/some-useful-tools-for-writing-react'>Some Useful Tools for Writing React</a> on Learn.co and start learning to code for free.</p>
