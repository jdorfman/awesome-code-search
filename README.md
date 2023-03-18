# Awesome Code Search [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome code search queries (_Sourcegraph, GitHub, grep.app, etc._) that make developers more productive.

## Contents
* [Security](#security)
* [TypeScript](#typescript)
* [Golang](#golang)
* [Docker](#docker)

## Security
* [RSA, DSA, EC, and PGP private keys](https://sourcegraph.com/search?q=-----BEGIN+%28RSA%7CDSA%7CEC%7CPGP%29+PRIVATE+KEY-----&patternType=regexp&sm=0)
* [Generic Secret](https://sourcegraph.com/search?q=context:global+%5BsS%5D%5BeE%5D%5BcC%5D%5BrR%5D%5BeE%5D%5BtT%5D.*%5B%27%7C%5C%22%5D%5B0-9a-zA-Z%5D%7B32%2C45%7D%5B%27%7C%5C%22%5D&patternType=regexp&sm=1&groupBy=repo)
* [Generic API Key](https://sourcegraph.com/search?q=context:global+%5BaA%5D%5BpP%5D%5BiI%5D_%3F%5BkK%5D%5BeE%5D%5ByY%5D.*%5B%27%7C%5C%22%5D%5B0-9a-zA-Z%5D%7B32%2C45%7D%5B%27%7C%5C%22%5D&patternType=regexp&sm=1&groupBy=repo)
* Find log4j dependencies across all your code ([Gradle](https://sourcegraph.com/search?q=org%5C.apache%5C.logging%5C.log4j%27+2%5C.%28%280%7C1%7C2%7C3%7C4%7C5%7C6%7C7%7C8%7C9%7C10%7C11%7C12%7C13%7C14%7C15%29%28%5C.%5B0-9%5D%2B%29%29+%0Alang:gradle+count:all&patternType=regexp&sm=0), [Maven](https://sourcegraph.com/search?q=%3Clog4j%5C.version%3E2%5C.%28%280%7C1%7C2%7C3%7C4%7C5%7C6%7C7%7C8%7C9%7C10%7C11%7C12%7C13%7C14%7C15%29%28%5C.%5B0-9%5D%2B%29%29%3C/log4j%5C.version%3E+%0Afile:pom%5C.xml&patternType=regexp&sm=0), [Ivy](https://sourcegraph.com/search?q=org%3D%22org%5C.apache%5C.logging%5C.log4j%22.*rev%3D%222%5C.%28%280%7C1%7C2%7C3%7C4%7C5%7C6%7C7%7C8%7C9%7C10%7C11%7C12%7C13%7C14%7C15%29%28%5C.%5B0-9%5D%2B%29%29%22+%0Afile:ivy%5C.xml+count:all&patternType=regexp&sm=0), [Scala](https://sourcegraph.com/search?q=%22org.apache.logging.log4j%22+%25+%222.%28%280%7C1%7C2%7C3%7C4%7C5%7C6%7C7%7C8%7C9%7C10%7C11%7C12%7C13%7C14%7C15%29%28%5C.%5B0-9%5D%2B%29%29%0Afile:%5C.sbt%24+count:all&patternType=regexp&sm=0), [Bazel](https://sourcegraph.com/search?q=org%5C.apache%5C.logging%5C.log4j:+2.%28%280%7C1%7C2%7C3%7C4%7C5%7C6%7C7%7C8%7C9%7C10%7C11%7C12%7C13%7C14%7C15%29%28%5C.%5B0-9%5D%2B%29%29%0Alang:bazel+count:all&patternType=regexp&sm=0))

## TypeScript
* [Find function overloads](https://sourcegraph.com/search?q=%5Efunction+%5Ba-zA-Z%5D%2B%5C%28.%2B%5C%29%3A+%5Ba-zA-Z%5D%2B%3B%24+lang%3ATypeScript+not+path%3A%5C.d%5C.ts%24&patternType=regexp&sm=0&groupBy=repo)

## Golang
* [Find all Go functions that contain "compile"](https://sourcegraph.com/search?q=r%3Agolang%2Fgo+compile+type%3Asymbol+select%3Asymbol.function&patternType=standard&sm=0&groupBy=repo)

## Docker
* [Repos with a Dockerfile](https://sourcegraph.com/search?q=context:global+repo:has.file%28Dockerfile%29&patternType=standard&sm=0&groupBy=repo)