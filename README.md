# jql-query-active-users

![Build Status](https://img.shields.io/travis/clef/jql-query-active-users.svg)
![Downloads](https://img.shields.io/npm/dm/@clef/jql-query-active-users.svg)
![Downloads](https://img.shields.io/npm/dt/@clef/jql-query-active-users.svg)
![npm version](https://img.shields.io/npm/v/@clef/jql-query-active-users.svg)
![dependencies](https://img.shields.io/david/clef/jql-query-active-users.svg)
![dev dependencies](https://img.shields.io/david/dev/clef/jql-query-active-users.svg)
![License](https://img.shields.io/github/license/clef/jql-query-active-users.svg)

A Mixpanel JQL query to measure active users

## Installation

Install it via npm:

```shell
npm install @clef/jql-query-active-users
```

## Usage

```javascript
import ActiveUsersQuery from '@clef/jql-query-active-users';

MP.api.jql(
  ActiveUsersQuery,
  {
    fromDate: moment().subtract(20, 'days').toDate(),
    toDate: moment().toDate(),
    events: []
  }
).done((results) => {
  console.log(results)
})
```

## Development

To start development, run:

```shell
git clone git@github.com:clef/jql-query-active-users.git jql-query-active-users
cd jql-query-active-users
npm install
npm run test
```


## License

MIT
