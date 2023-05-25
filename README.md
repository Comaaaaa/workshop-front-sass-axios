## 1. Set Up a React Project:
Create a new React project using the create-react-app utility:

This command creates a new React application with a modern, out-of-the-box setup, which includes a live development server, Jest for testing, and more.```
```
npx create-react-app your_project_name
cd your_project_name
```

## 2. Install Axios:
Axios is a popular, promise-based HTTP client that sports an easy-to-use API and can be used in both the browser and Node.js.

Sass (Syntactically Awesome Style Sheets) is a CSS preprocessor, which allows you to use variables, nested rules, mixins, functions, and more, all with a fully CSS-compatible syntax.
```bash
npm install axios
```

## 3. Create Components:
In your React project, you'll create various components. Remember to place these components in the src/components directory.

A component is a reusable piece of your website. It could be a button, a form, a section of a page, or even the entire page itself.

## 4. Make API Requests:
You'll use Axios to communicate with your API. To do so, import Axios at the top of your component file:

Axios provides a simple to use library in which we can send asynchronous HTTP request to REST endpoints and perform CRUD operations.
```
import axios from 'axios';
```
You'll use Axios to send requests to your API, like so:

```
const response = await axios.get('/yourAPI/yourRoute');
```
Make sure to handle the response and potential errors appropriately.


## 5. Style the Components:
For each component, you'll create a Sass file in the same directory as the component. Import it at the top of your component file:

Sass provides a more robust framework for working with CSS, including features like variables, nesting, and mixins, which can make your stylesheets more readable and maintainable.

```
import './ComponentName.scss';
```
Here are a few things you can do with Sass:

* Variables: Sass variables start with a `$` and make it easy to reuse CSS properties throughout your stylesheet.

* Nesting: Sass allows you to nest your CSS selectors, making your styles more organized and maintainable.

* Mixins: Think of mixins as functions for CSS. You define a set of styles once, and then you can "mix" them in wherever you need to.

* Functions: Sass also provides a variety of functions that can be used to manipulate colors, strings, and numbers.

Then, apply the styles to the corresponding HTML elements in the component.

## 6. Render Components:

In your src/index.js file, you'll import your main component and render it. Don't forget to use ```ReactDOM.render()```.

This is where you attach your root component to a DOM element. All of your other components will be children of this root component, forming a component tree.


![logo](https://user-images.githubusercontent.com/72024056/240905042-6f955418-df69-4bcc-8657-b4a4627899a3.png)

Your goal on this step is to try to make reusable components that will store different part of your datas and allow you to display it the way you want, in the exemple above, I am using the framework `recharts` and `MUI` that allows you to make some cool features and display informations in the case you need to display charts.

Feel free to use the methods you want

### DO NOT OVERLOAD YOUR index.js FILE !

They should normally look like this, it should not be too long because of your code must stay maintainable

```
import Whatever you need

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);
```

## 7. Test your project

Ensure that you adjust the API endpoint URLs and data handling code based on your specific API implementation.

Finally, start the development server and view your React app in the browser:
```bash
npm start
```

Your React app should now be running and fetching data from your API, with styling applied to the components.