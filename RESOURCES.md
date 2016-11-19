Before getting started with the project, please take some time to read *and* understand the following articles:

*   [Displaying data with JSX](https://facebook.github.io/react/docs/displaying-data.html)

*   [JSX in depth](https://facebook.github.io/react/docs/jsx-in-depth.html)

*   [Interactivity and dynamic UIs](https://facebook.github.io/react/docs/interactivity-and-dynamic-uis.html)

*   [Multiple components](https://facebook.github.io/react/docs/multiple-components.html)

*   [The React way: getting started tutorial](https://blog.risingstack.com/the-react-way-getting-started-tutorial/)

    **NOTE**: we will not be building a so-called "isomorphic" application so you may skip that part of the article.

*   [Five practical examples for learning React](http://tutorialzine.com/2014/07/5-practical-examples-for-learning-facebooks-react-framework/)

    **NOTE**: make sure to reproduce each of the five examples on your own!

    **NOTE 2**: in the last example, the tutorial uses jQuery to do AJAX. Try to do it with [`isomorphic-fetch`](https://github.com/matthew-andrews/isomorphic-fetch)

*   [Introduction to `react-router`](https://github.com/reactjs/react-router/blob/master/docs/Introduction.md)

    **NOTE**: routing is a concept you are already familiar with, but on the server side.

    As far as we are concerned, routing is the process of deciding what to display based on the current URL.

    On the server side, we are using the Express library to help us do our routing. For example, we tell Express that we want to handle **`GET`** requests to `/content/:id`. When a request comes along for this URL, Express knows which function to call.

    Routing in the browser is similar: we already saw that we could induce a change of the URL in the browser without refreshing the page, by using the [History API](https://developer.mozilla.org/en-US/docs/Web/API/History_API) provided by the browser. Similarly, [we can get notified when the URL changes](https://developer.mozilla.org/en-US/docs/Web/API/WindowEventHandlers/onpopstate) due to the back or forward buttons being clicked.

    If we put these two concepts together, we can write JavaScript code for the browser that can decide what to display based on the current URL. We can do it manually, but `react-router` does it for us :)

* [React router: a comprehensive introduction](https://www.themarketingtechnologist.co/react-router-an-introduction/)