redux-create-reducer
===

[![NPM version][npm-image]][npm-url]
[![Build status][travis-image]][travis-url]
[![Test coverage][coveralls-image]][coveralls-url]
[![Downloads][downloads-image]][downloads-url]

[This code packaged as a node module](https://github.com/rackt/redux/blob/9b0630fe9ea8209777fed7cac78fee7ee76fce67/docs/recipes/ReducingBoilerplate.md#generating-reducers)

Usage:

```js
import { createReducer } from 'redux-create-reducer';
import * as ActionTypes from '../constants/ActionTypes';

const initialState = [];


export const todos = createReducer(initialState, {
  [ActionTypes.ADD_TODO](state, action) {
    let text = action.text.trim();
    return [...state, text];
  }
})
```



[npm-image]: https://img.shields.io/npm/v/redux-create-reducer.svg?style=flat-square
[npm-url]: https://npmjs.org/package/redux-create-reducer
[travis-image]: https://img.shields.io/travis/kolodny/redux-create-reducer.svg?style=flat-square
[travis-url]: https://travis-ci.org/kolodny/redux-create-reducer
[coveralls-image]: https://img.shields.io/coveralls/kolodny/redux-create-reducer.svg?style=flat-square
[coveralls-url]: https://coveralls.io/r/kolodny/redux-create-reducer
[downloads-image]: http://img.shields.io/npm/dm/redux-create-reducer.svg?style=flat-square
[downloads-url]: https://npmjs.org/package/redux-create-reducer
