---
title: Actions
description: Akcje oraz ich pomoc w manipulacji stanem w Gatsby
jsdoc:
  - "gatsby/src/redux/actions/public.js"
  - "gatsby/src/redux/actions/restricted.js"
contentsHeading: Functions
---

Gatsby wewnętrznie wykorzystuje [Redux](http://redux.js.org) do zarządzania stanem. Kiedy implementujesz Gatsby API, przechodzisz przez zbiór akcji (odpowiednik powiązywania akcji [bindActionCreators](https://redux.js.org/api/bindactioncreators/) w Redux), które możesz wykorzystać do manipulacji stanem na swojej stronie.

Obiekt `actions` zawiera funkcje, które mogą być indywidualnie destrukturyzowane za pomocą składni ES6 ([destrukturyzacja obiektów](https://developer.mozilla.org/pl/docs/Web/JavaScript/Referencje/Operatory/Destructuring_assignment#Destrukturyzacja_obiekt%C3%B3w)).

```javascript
// Dla funkcji createNodeField
exports.onCreateNode = ({ node, getNode, actions }) => {
  const { createNodeField } = actions
}
```
