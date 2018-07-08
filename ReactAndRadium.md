# The best “styling in React” tutorial you’ve ever seen
## Inline styling
## Styled Components
## CSS Modules

https://blog.logrocket.com/the-best-styling-in-react-tutorial-youve-ever-seen-676f1284b945

# React Inline Styles 
video
React Inline Styles and ReactJS instead of CSS
https://youtu.be/k3OF4A30jSQ

* Specificity Hell

More specific rule: a {color: orange} vs .headerClass a {color: white}

Moving components, specificity can create UI issues. A css senior can refactor with more general rules. 

* Source Order Woes

If two components have the same specificity, the last one to appear wins. In large apps this can easily happen.

* Naming Collisions

Large proj, you ran of good class names quickly.

css selector is global, hard to keep track

Solutions:
naming conventions,
practice code review,
and search code base thoroughly

* Dead Code

 Difficult to remove old css. It's dangerous to remove it.
 
 # React
 * Server and client. Not only in browser anymore.
 * One way data flow model, simple structure than MVC
 * Everything is a component. Encapsulates and makes them consistent, readable and maintainable.

Abandon JS entirely and managing styles with JS instead. 

# Radium library
A toolset for managing inline styles with react. Makes it easier to write css.

React built in inline styles support

Most React apps are written in JSX. Creating markup (text) with javascript using html like syntax.

React feature of groups of styles properties using JS Objects and use them as inline styles in a component using braces.

## Benefits
* Variables
* No specifity, flat as possible
* Source order independence. Scoped to component
* Naming: Styles are scoped to module
* Dead code elimination: Remove component, styles are gone.

Styles are isolated and encapsulated, much easier to change and maintain vs css.

## Radium features
* Browser states ex :hover inside js object style
* Media queries: Inside obj sytle
* Style arrays: An array of styles objs style = {[styles.base, styles.base2]} kind of like class="btn btn-primary"
React styles have to be a JS obj single level deep and flat

React Virtual DOM: React app creates obj tree to represent your current DOM.
Diffing allows react to make the smallest possible change.
