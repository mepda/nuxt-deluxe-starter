# nuxt-deluxe-starter

## Welcome!

The point of this repo is to achieve two things:

1. Make an opensource template encompassing basic essentials of all webapps in Nuxt. Such as...

   - Responsive Navbar
   - Effects, like AOS, animate.css, etc
   - State and stateful transactions
   - Authentication (if not implemented in the repo, then really clear instructions on how to get this set up with services like AWS Amplify)
   - Maps
   - Graphs / Charts

2. Document and explain clearly all the functionalities of what's been put inside this app
   - So for things like the vuex store, there's a detailed yet concise explanation of how various actions / getters / mutations are used and what a general way to call them is
   - Links to further reading and explanations are listed when appropriate

## Contributing and Style guidelines

I'd like for this repo to follow two CSS rules

    1. Bulma classes
    2. BEM classes

For all logic use the following rules:

    1. Variable names should use camelCase.
    2. Document all functions and functionality.

For making pull requests, assign yourself to an issue and then make a PR against the master branch

## Build Setup (Nuxt pregenerated MD)

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
