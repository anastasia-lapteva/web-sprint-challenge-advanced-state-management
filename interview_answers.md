# Interview Answers
Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?

React Context API is a way for React app to produce global variables that can be passed around. It helps to avoid "prop drilling," which is moving props from grandparents to parents to children, etc. Context API allows for a way to share values between components without having to pass a prop through every single level of the tree.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

`Store` is what holds all the data that your application uses, which is why it's known as a 'single source of truth'. Components using data from teh Store will re-render themselves when the data changes.
`Actions` are JavaScript objects that indicate what should be performed (they describe what happens). Actions carry payloads of information from your application to the store.
`Reducers` are functions that take an action and the previous state of the application, and return a new state based on that action.

3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?

`redux-thunk` is a middleware for React Redux. It allows you to write `action-creators` that return a function instead of an action. This function that returns a function is called a thunk.

4. What is your favorite state management system you've learned and this sprint? Please explain why!

My favorite state management system that I've learned this sprint is Redux because of the STORE! I think it's so great you don't have to drag values through pages of props because at times it becomes confusing in regards to where these props are even coming from.