// const heading = React.createElement(
//   "h1",
//   { id: "heading" },
//   "Hello World from React!"
// );
// const root = ReactDOM.createRoot(document.getElementById("root"));
// root.render(heading);

//Nested tag Example
/*
 * <div>
 *      <div>
 *          <h1> Hello World for Nested Tag in React</h1>
 *      </div>
 * </div>
 *
 * 
 */

const parent = React.createElement(
  "div",
  { id: "parent" },
  React.createElement(
    "div",
    { id: "child" },
    React.createElement(
      "h1",
      { id: "heading" },
      "Hello World for Nested Tag in React"
    )
  )
);
const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(parent);
