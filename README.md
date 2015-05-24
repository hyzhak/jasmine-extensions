# jasmine-extensions
Matchers and helpers for jasmine

## Extension

* [github.com/hyzhak/jasmine-es6-generator](https://github.com/hyzhak/jasmine-es6-generator)
  helps to tests generators as async function
  
  ```javascript
  var gen = require('jasmine-es6-generator');
  
  it('should done', gen(function *() {
    var res = yield someFn();
    expect(res).toEqual(1234);
  }));
  ```

## Matchers

* https://github.com/bvaughn/jasmine-es6-promise-matchers test whether result of promise will be certain value
  
  ```javascript
  expect(promise).toBeResolvedWith('something', done);
  ```
  
* https://github.com/hyzhak/to-have-property test whether object has projerty (with certain value)
  
  ```javascript
  expect({ y: 123}).toHaveProperty('y', 123);
  expect({ x: 1, y: 2, z: 3}).toHaveProperties({'x': 1, 'y': 2});
  ```
  
* https://github.com/hyzhak/to-have-method test whether object has method
 
  ```javascript
  expect({ m: function() {} }).toHaveProperty('m');
  expect({ m1: function() {}, m2: function() {} }).toHaveMethods('m1', 'm2');
  ```
  
  [test](test)
  [/test](/test)
  [/test.md](/test.md)
  [/test.html](/test.html)
