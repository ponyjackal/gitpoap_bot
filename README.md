# gitpoap-bot

The GitPOAP bot is a GitHub App built with [Probot](https://github.com/probot/probot) with two main functions:
 - [GitPOAP Notifications](https://docs.gitpoap.io/github-bot): a feature to notify users when a contribution has earned them a GitPOAP on opted-in & supported repositories
 - [Ad-hoc GitPOAP awards](https://docs.gitpoap.io/github-bot#tagging-contributors): the ability for a maintainer to tag users ad-hoc on an Issue or Pull Request who should be awarded a GitPOAP


## Setup

```sh
# Install dependencies
yarn

# Build the typescript code
yarn build

# Run the bot
yarn start
```

## Docker

```sh
# 1. Build container
docker build -t gitpoap-bot .

# 2. Start container
docker run -e APP_ID=<app-id> -e PRIVATE_KEY=<pem-value> gitpoap-bot
```

## Contributing

If you have suggestions for how gitpoap-bot could be improved, or want to report a bug, open an issue! We'd love all and any contributions.

For more, check out the [Contributing Guide](CONTRIBUTING.md).

## License

[ISC](LICENSE) © 2022 Jay Puntham-Baker <jay@gitpoap.io>
