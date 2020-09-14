# Book Buddy

A microservice for looking up book information by ISBN.

Complies to the [JSON API Spec](https://jsonapi.org/).

## Versions

sinatra (2.1.0)

ruby 2.5.3

## Setup and Installation

## Usage and Endpoints

Search for a book by ISBN_13

`GET /search?isbn=<YOUR_BOOK_ISBN>`

### Example Request and Response

`GET /search?isbn=9781775417415`

```JSON
{
  "data": {
    "id": null,
    "type": "book",
    "attributes": {
      "title": "The Wings of the Dove",
      "author": "Henry James",
      "description": "Young Londoners Kate and Merton are engaged, but have no money to marry on. When the wealthy but terminally ill American heiress Milly arrives in London, Kate schemes for a way to inherit her fortune. But when Kate achieves all she had hoped for, she finds that the money and the gentle, beautiful Milly have changed everything.",
      "thumbnail": "http://books.google.com/books/content?id=iTeEpRJogFMC&printsec=frontcover&img=1&zoom=1&edge=curl&source=gbs_api",
      "isbn": "9781775417415",
      "category": "Fiction"
    }
  }
}
```
