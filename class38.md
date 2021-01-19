# React

## Conditional rendering


#### Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.


![f](https://colorlib.com/wp/wp-content/uploads/sites/2/react-dev-tools-logo.jpg)


Preventing Component from Rendering
In rare cases you might want a component to hide itself even though it was rendered by another component. To do this return null instead of its render output.

In the example below, the <WarningBanner /> is rendered depending on the value of the prop called warn. If the value of the prop is false, then the component does not render.



### Keys
Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity

![s](https://cmichel.io/static/8b84cc2f38f0ee541e61c9788149e14d/eb2af/react-keys-index.png)
