# Initial Setup

### Initialize the project

```
npm-init -y
```

### Getting Eslint and Config

First install Eslint - Prettier

```
npm i -D eslint prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-node eslint-config-node
```

Next the Airbnb config

```
npx install-peerdeps --dev eslint-config-airbnb
```

Create a new file called `.prettierrc` and include the next lines:

```
{
 "singleQuote": true
}
```

Now, it's time to get Eslint ready, run:

```
sudo npm i eslint
```

And initialize Eslint with:

```
eslint --init
```

Override the content in `.eslint.json` and include the following:

```
{
 "extends": ["airbnb", "prettier"],
 "plugins": ["prettier"],
 "rules": {
	"prettier/prettier": "error",
	"no-unused-vars": "warn"
	}
}
```
