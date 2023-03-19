# Electrify Chicago

[![Netlify Status](https://api.netlify.com/api/v1/badges/d777babe-6135-45a1-99dd-6377999b6127/deploy-status)](https://app.netlify.com/sites/radiant-cucurucho-d09bae/deploys)

A site to publicize some of the most polluting buildings based on the Chicago Energy Benchmarking data published in the City of Chicago Data Portal.

## Data Import

Sources:

- [Chicago Energy Benchmarking - Covered Buildings Data](https://data.cityofchicago.org/Environment-Sustainable-Development/Chicago-Energy-Benchmarking-Covered-Buildings/g5i5-yz37)

### Cleanup

GraphQL requires data key names to have no spaces or special characters, so there's a raw data file (only filtered by GHG emissions > 1,000 tons and year = 2020) and a cleaned file that just hast he headers renamed for GraphQL.

## To-Do List

- [x] Pick a framework - statically built VueJSS, maybe [VitePress](https://vitepress.dev/guide/getting-started)
- [x] Setup landing page with SCSS working
- [x] Get CSV data usable and on homepage
- [x] Setup domain and build process
- [ ] Setup unit tests
- [ ] Setup linting (ESLint, Prettier, Stylelint)
- [ ] Setup Typescript

## Development

## Setup

Make sure you have [Yarn](https://yarnpkg.com/) installed, `cd` into the project directory (after cloning it) and run:

```
yarn install
```

## Running

Run `yarn develop` to start a local dev server at `http://localhost:8080`

Happy coding 🎉🙌

## Run Linting

Run:

```
yarn lint-fix
```

## Deploys

This site deploys automatically via Netlify by running `gridsome build`.
