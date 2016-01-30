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
Get list of books.
```javascript
HttpRequest.get('/books')
  .then(function (response) {
    // Get list of books in response
  })
  .catch(function () {
    // Handle error response
  });
```

#### post
Create new book.
```javascript
var book = {
  // book fields go here
};
HttpRequest.post('/books', book)
  .then(function (response) {
    // Get successful response
  })
  .catch(function () {
    // Handle error response
  });
```

#### put
Update existing book.
```javascript
var book = {
  // book fields go here
};
HttpRequest.put('/books/123', book)
  .then(function (response) {
    // Get successful response
  })
  .catch(function () {
    // Handle error response
  });
```

#### delete
Delete one book.
```javascript
HttpRequest.delete('/books/123')
  .then(function (response) {
    // Get successful response
  })
  .catch(function () {
    // Handle error response
  });
```

#### patch
Update specific parts of the book.
```javascript
var book = {
  // book fields go here
};
HttpRequest.patch('/books/123', book)
  .then(function (response) {
    // Get successful response
  })
  .catch(function () {
    // Handle error response
  });
```

#### trace
```javascript
HttpRequest.trace('/books')
  .then(function (response) {
    // Get successful response
  })
  .catch(function () {
    // Handle error response
  });
```

#### options
```javascript
HttpRequest.options('/books')
  .then(function (response) {
    // Get successful response
  })
  .catch(function () {
    // Handle error response
  });
```

#### head
```javascript
HttpRequest.head('/books', book)
  .then(function (response) {
    // Get successful response
  })
  .catch(function () {
    // Handle error response
  });
```
