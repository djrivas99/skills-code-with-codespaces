### You are learning about codespaces!
name: Step 1, Create codespace and push code
# This step triggers after push to main.
# This workflow updates from step 1 to step 2.

on# This will run every time we push to main.
# Reference: https://docs.github.com/en/actions/learn-github-actions/events-that-trigger-workflows
on:
  workflow_dispatch:
  push:
    branches:
      - main
    jobs:
        build:
            runs-on: ubuntu-latest

            steps:
                - name: Checkout code
                    uses: actions/checkout@v2

                - name: Set up Node.js
                    uses: actions/setup-node@v2
                    with:
                        node-version: '14'

                - name: Install dependencies
                    run: npm install

                - name: Build project
                    run: npm run build

                - name: Deploy to GitHub Pages
                    run: npm run deploy
                    