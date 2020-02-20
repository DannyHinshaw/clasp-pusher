# Clasp Pusher

Simple too for pushing new production releases to the Google Docs "production document".

## Setup

Git clone this repo locally.

Reference to Google Clasp CLI: https://github.com/google/clasp

## Steps:

1. Fill out the `.clasp.json` file with the correct "production document" script id.

2. You may need to login with clasp:
    ```bash
    yarn clasp:login
    ```

2. From terminal (in project root), run:

    ```bash
    yarn clasp:push
    ```

That's it!
