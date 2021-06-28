# Configuration

## Prerequisites

1) Install Node.js (https://nodejs.org/)

## Integration into the TypeScript project

2) Add development dependencies

```
npm install typescript eslint prettier eslint-config-prettier @typescript-eslint/parser @typescript-eslint/eslint-plugin -D
```

3) Add **.eslintrc**, **.eslintignore**, **.prettierrc**, **.prettierignore** files into root project folder

## Add scripts

4) Add scripts to the **package.json** file

```
{
    ...
    "scripts": {
        ...
        "format": "prettier --write \"src/**/*.{ts,js}\" \"tests/**/*.test.ts\"",
        "lint": "eslint \"src/**/*.{ts,js}\" --fix",
        ...
    },
    ...
}
```

# Using

## To check code quality

```
npm run lint
```

## To format code

```
npm run format
```
