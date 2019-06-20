# snips-action-reminder

Snips action code for the Reminder app

## Setup

```sh
sh setup.sh
```

Don't forget to edit the `config.ini` file.

An assistant containing the intents listed below must be installed on your system. Deploy it following [these instructions](https://docs.snips.ai/articles/console/actions/deploy-your-assistant).

## Run

- Dev mode:

```sh
# Dev mode watches for file changes and restarts the action.
npm run dev
```

- Prod mode:

```sh
# 1) Lint, transpile and test.
npm start
# 2) Run the action.
node action-snips.js
```

## Test & Demo cases

This app only supports french 🇫🇷 and english 🇬🇧.

## Debug

In the `src/index.ts` file:

```js
// Uncomment this line to print everything
// debug.enable(name + ':*')
```

## Test & Lint

*Requires [mosquitto](https://mosquitto.org/download/) to be installed.*

```sh
npm start
```

**In test mode, i18n output and http calls are mocked.**

- **http**: mocks are written in `tests/httpMocks/index.ts`
- **i18n**: mocked by `snips-toolkit`, see the [documentation](https://github.com/snipsco/snips-javascript-toolkit#i18n).

## Contributing

Please see the [Contribution Guidelines](https://github.com/snipsco/snips-action-reminder/blob/master/CONTRIBUTING.md).

## Copyright

This library is provided by [Snips](https://snips.ai) as Open Source software. See [LICENSE](https://github.com/snipsco/snips-action-reminder/blob/master/LICENSE) for more information.
