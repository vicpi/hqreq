# HQReq - Library for making AJAX requests

## Installation

Using npm:

```bash
$ npm install --save hqreq
```

## Usage

#### Import HttpRequest
ES6 modules
```
import {HttpRequest} from 'hqreq';
```
Browserify
```
var HttpRequest = require('hqreq').HttpRequest;
```

#### get
```javascript
HttpRequest.get('/books')
  .then(function (response) {
    // get list of books in response
  })
  .catch(function () {
    // Handle error response
  });
```

#### post
```javascript
var book = {
  // book fields go here
};
HttpRequest.post('/books', book)
  .then(function (response) {
    // create new book
    // get successful response after creating new book
  })
  .catch(function () {
    // Handle error response
  });
```

#### put
```javascript
var book = {
  // book fields go here
};
HttpRequest.put('/books/123', book)
  .then(function (response) {
    // update existing book
    // get successful response
  })
  .catch(function () {
    // Handle error response
  });
```

#### delete
```javascript
HttpRequest.delete('/books/123')
  .then(function (response) {
    // delete one book
    // get successful response
  })
  .catch(function () {
    // Handle error response
  });
```

#### patch
```javascript
var book = {
  // book fields go here
};
HttpRequest.patch('/books/123', book)
  .then(function (response) {
    // update specific parts of the book
    // get successful response
  })
  .catch(function () {
    // Handle error response
  });
```

#### trace
```javascript
HttpRequest.trace('/books')
  .then(function (response) {
    // get successful response
  })
  .catch(function () {
    // Handle error response
  });
```

#### options
```javascript
HttpRequest.options('/books')
  .then(function (response) {
    // get successful response
  })
  .catch(function () {
    // Handle error response
  });
```

#### head
```javascript
HttpRequest.head('/books', book)
  .then(function (response) {
    // get successful response
  })
  .catch(function () {
    // Handle error response
  });
```
