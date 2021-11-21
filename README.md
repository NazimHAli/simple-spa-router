# simple-spa-router-ts
Basic router written in one class. Useful for small projects/prototyping.

## Example

```javascript

import Router from "router";

const router = new Router({
    mode: "hash",  // hash or history
    root: "/",
});

// Add routes + logic to handle route changes
router
    .addRoute(/about/, () => {
        // Route to about page: /#/about/
    })
    .addRoute(/blog\/post/, () => {
        // Regex to handle all URLs starting with /#/blog/post/
    })
    .addRoute("", () => {
        // Route to homepage: /#/
    });

```