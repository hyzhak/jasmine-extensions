# jasmine-extensions
Matchers and helpers for jasmine

# Matchers

* https://github.com/bvaughn/jasmine-es6-promise-matchers test whether result of promise will be certain value
  ```javascript
  expect(promise).toBeResolvedWith('something', done);
  ```
  
* https://github.com/hyzhak/to-have-property test whether object has projerty (with certain value)
  ```javascript
  expect({ y: 123}).toHaveProperty('y', 123);
  ```
* https://github.com/hyzhak/to-have-method test whether object has method
  ```javascript
  expect({ m: function() {} }).toHaveProperty('m');
  ```
