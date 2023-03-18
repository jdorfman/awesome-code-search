# Awesome Code Search [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome code search queries (Sourcegraph, GitHub, grep.app, etc.) that make developers more productive.

## Contents
* [Security](#security)
* [TypeScript](#typescript)

## Security
* [Search for RSA, DSA, EC, and PGP private keys](https://sourcegraph.com/search?q=-----BEGIN+%28RSA%7CDSA%7CEC%7CPGP%29+PRIVATE+KEY-----&patternType=regexp&sm=0)

## TypeScript
* [Find function overloads](https://sourcegraph.com/search?q=%5Efunction+%5Ba-zA-Z%5D%2B%5C%28.%2B%5C%29%3A+%5Ba-zA-Z%5D%2B%3B%24+lang%3ATypeScript+not+path%3A%5C.d%5C.ts%24&patternType=regexp&sm=0&groupBy=repo)
