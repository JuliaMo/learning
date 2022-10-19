# RICOH360 Website
## this is a test

Website for RICOH360

## Requirements

- Node.js `14.x` with [Yarn](https://yarnpkg.com): `$ brew install yarn`

## Getting Started

Install dependencies:

```
yarn
```

Start development server:

```
yarn develop
```

Open with your browser:

```
open http://localhost:8000
```

## Development

### Start development server

```
yarn develop
```

### Clean

```
yarn clean
```

### Debug build-time with node inspector

```
yarn debug
```

### Debug run-time with node inspector

Using the menu `Run > Start Debugging` from VS Code after `yarn develop` or `yarn debug`

### Create production build and serve locally

```
yarn build && yarn serve
```

## Run E2E test on local

Copy environment files:

```
cp .env.example .env.development
cp .env.example .env.production
```

Build:

```
yarn build
```

Serve it on port 8000:

```
yarn serve -p 8000

// or the following command doesn't demand you to copy .env.development

NODE_ENV=production yarn serve -p 8000
```

Run Cypress:

```
yarn cy:run
```

## Check website for specific region on Localhost

Make sure you already copied `.env.development` from `.env.example`. if not, run this command,

```
cp .env.example .env.development
```

Specify the environment variable `COUNTRY=` in `.env.development` file. For example, if you want to check the website for Japan, set `COUNTRY=jp` in `.env.development` file.
Available regions are the followings:

- jp
- us
- eu

Run dev server:  
(_highly recommend to run `yarn clean` before running dev server._)

```
yarn start
```
## this is a test
