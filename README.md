# jest-runner-write-good

A jest runner that "lints" your text with [write good](https://github.com/btford/write-good) to check if your language seems nice and clean.

## Installation

0. Have jest setup
1. Run `npm install --save-dev jest-runner-write-good`
2. Add this to your jest config

```json
{
    "jest": {
        "projects": [{
            "displayName": "Write Good",
            "transform": {
                ".md$": "md-to-text" // Do I need this?
            },
            "testMatch": ["**/*.md", "**/*.txt"],
            "runner": "jest-runner-write-good"
        }]
    }
}
```

3. Run `npm test`

## TODO

- [ ] check if we can use markdown directly
- [ ] implement POC

