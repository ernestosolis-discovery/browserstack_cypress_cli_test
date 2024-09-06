### Intro
This Project is based on the cypress kitchen sink project as a standalone agnostic project that has no reference to 
a real application and data.
The main purpose is to test capabilities and integrations without compromising any real project or data.

The project currently integrates with browserstack cypress cli tool which allows
the project to be run on the browserstack cloud testing environment, in order to test their capabilities.

### References:

#### Cypress docs:
https://docs.cypress.io/examples/applications#Kitchen-Sink

#### Github repo:
https://github.com/cypress-io/cypress-example-kitchensink


#### Browserstack cypress CLI docs:
https://www.browserstack.com/docs/automate/cypress

#### Browserstack cypress CLI repo:
https://github.com/browserstack/browserstack-cypress-cli?tab=readme-ov-file

#### Browserstack download custom reports:
https://www.browserstack.com/docs/automate/cypress/custom-reports-build-artifacts#download-custom-reports

### Setup:
Install dependencies:
```npm i
```
Install browserstack cli:
`npm i -g browserstack-cypress`

### Authenticate with browserstack


Define the required env vars for browserstack
replace the values in the following commands
or set them the way you prefer

```
export BROWSERSTACK_USERNAME=your_username
export BROWSERSTACK_ACCESS_KEY=your_accesskey
```

## Commands to run the tests:

### Run tests locally
Run all of the tests:
```
npm run test
```
The Reports will be located under `mochawesome-report`

Run only one spec file:
```
npm run test-single-test
```

### Run tests on browserstack

Run all  the tests in browserstack:
```
npm run test-browserstack
```

Run one test in browserstack:
```
npm run test-browserstack-single-test
```

Run one test in browserstack with the reporter options:
```
npm run test-browserstack-reporter-single-test
```
