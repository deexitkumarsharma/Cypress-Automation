# Cypress-Automation

This repo contains end-to-end tests written in Cypress for the shopist.io application.

## Run Tests

To run cart actions tests in interactive mode use following command

`npx cypress open`

To run cart actions tests in normal mode use following command

`npm run cy:run-all`

## Demo

![App Screenshot](cypress/screenshots/Screenshot%20from%202023-01-25%2015-40-50.png))

## Patterns

Despite what Cypress says, the page object model is used because it improves code readability.

- POM pattern is used, and every page at [shopist.io] (https://www.shopist.io) is represented as a single class.
- Fixtures > profileDetails.json provides data.

## Dependencies

    "cypress": "^12.4.0",
    "cypress-file-upload": "^5.0.8",
    "cypress-mochawesome-reporter": "^3.2.3",
    "mocha": "^10.2.0",
    "mochawesome": "^7.1.3",
    "mochawesome-merge": "^4.2.2"

## Lessons Learned

It's common to mix up synchronised Cypress and asynchronous Javascript codes.

Trying to prevent this from happening while chaining my assertions is a little challenging.

But binding elements to variables using `.then()` solved most of my issues.

## Feedback

If you have any feedback, please reach out to us at deexitkumarsharma@gmail.com
