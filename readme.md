# github-remove-forks [![Build Status](https://travis-ci.org/kevva/github-remove-forks.svg?branch=master)](https://travis-ci.org/kevva/github-remove-forks)

> Remove all forked repositories


## Install

```
$ npm install --save github-remove-forks
```


## Usage

```js
const githubRemoveForks = require('github-remove-forks');

githubRemoveForks({token: '523ef691191'}).then(data => {
	console.log('Successfully remove all forked repositories');
});
```


## API

### githubRemoveForks(options)

Returns a promise for an `array` with the removed repositories.

#### options

##### token

*Required*  
Type: `string`

Token to authenticate with. If you don't have a token you can generate a new one [here](https://github.com/settings/tokens/new).


## CLI

```sh
$ npm install --global github-remove-forks
```

```sh
$ github-remove-forks --help

  Usage
    $ github-remove-forks --token 523ef69119

  Options
    -t, --token      Github token to authenticate with
    -v, --verbose    Show detailed output
```


## Related

- [github-remove-all-releases](https://github.com/stevemao/github-remove-all-releases) - Remove all releases of a GitHub repo


## License

MIT © [Kevin Mårtensson](https://github.com/kevva)
