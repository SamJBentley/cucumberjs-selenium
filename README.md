# Headless Selenium & Cucumber JS with screenshots
### Summary
This uses the example given in [selenium-cucumber-js](https://www.npmjs.com/package/selenium-cucumber-js), instead using version 78 of ChromeDriver.

It runs BDD-style scenarios, defined in the Gherkin files, in the features folder. These are mapped to code, in the step-definitions folder, which control Chrome.

These tests can be executed with Chrome in GUI mode, or in headless mode. The headless mode executes in the project's [Travis CI](https://travis-ci.org/SamJBentley/cucumberjs-selenium).

### Screenshots
Test failures are automatically recorded with a screenshot, which can be viewed by looking at the reports folder

### Installation & run steps
1. Run `npm ci`. Do not run `npm install`, as the `package-lock.json` file has been converted into a `npm-shrinkwrap.json` file, as the Chromedriver dependency has been overridden. 
2. Add ChromeDriver to your PATH environment variable. This should be C:\Users\username\AppData\Local\Temp\78.0.3904.70\chromedriver
3. Run `npm test` for headless mode or `npm gui` for GUI mode