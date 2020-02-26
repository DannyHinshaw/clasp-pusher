# Clasp Pusher

Simple tool for pushing new production releases to the Google Docs "production document".

## Setup

1. Git clone this repo locally.

2. Install dependencies:

```bash
yarn
```

or

```bash
npm i
```

Reference to Google Clasp CLI: https://github.com/google/clasp


## Steps:

1. Drop in the release assets directory and make sure it's named `dist`
 (or rename the `rootDir` property in .clasp.json to match). 
 
    Project structure should look like:
    ```
   ├── clasp-pusher/
   |   ├── dist/ # Assets used for publishing to Chrome Web-Store.
   |   ├── node_modules/
   |   ├── .clasp.json/
   |   ├── .gitignore/
   |   ├── package.json/
   ...etc
    ```

2. Fill out the `.clasp.json` file with the correct "production document" script id.

3. You may need to login with clasp:
    ```bash
    yarn clasp:login
    ```
    or
    ```bash
    npm run clasp:login
    ```

4. From terminal (in project root), run:

    ```bash
    yarn clasp:push
    ```
    or
    ```bash
    npm run clasp:push
    ```
