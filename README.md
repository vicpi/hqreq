# HQReq

## Installation

Using npm:

```bash
$ npm install --save hqreq
```

## Usage

#### get
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


#### head

#### put

#### delete

#### trace

#### options

#### patch
