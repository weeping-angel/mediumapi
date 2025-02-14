# `medium-api-js`

This is a wrapper library designed to interact with Unofficial Medium API (mediumapi.com).

Medium (medium.com) is one of the biggest blogging platform on the planet. Medium API (Unofficial) helps developers fetch data from Medium's Website.

Using this library you can easily fetch data related to Medium articles, user, authors, publications, tags, lists, etc ...

## Installation

```shell
npm i medium-api-js
```

## Usage

```js
import Medium from 'medium-api-js';
require('dotenv').config();

const medium = new Medium(process.env.RAPIDAPI_KEY);

const userId = '6e2475a6e38a'; 

medium.getUserArticles(userId)
    .then(data => {
        console.log('User Articles:', data);
    })
```

> Note: You'll need to create a ".env" file and put your RAPIDAPI_KEY into it. Alternatively, you can set in your environment variables.

## How to Subscribe to Medium API and Get your API Key

See https://mediumapi.com/how-to-subscribe-to-medium-api.html

## Resources

- API Documentation: https://mediumapi.com/documentation.html
- Swagger Documentation: https://docs.mediumapi.com
- Frequently Asked Questions: https://mediumapi.com/frequently-asked-questions.html