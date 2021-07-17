#### Installing ESLint and Prettier locally

```bash
yarn add eslint prettier --dev
```

---

Add eslint plugin for react and react hooks

```bash
yarn add eslint-plugin-react eslint-plugin-react-hooks --dev
```

---

Create **.prettierrc** file inside root dir

```json
{
  "printWidth": 80,
  "trailingComma": "es5",
  "semi": true,
  "tabWidth": 2,
  "singleQuote": true
}
```

---

Creating **.eslintrc.json** file inside root dir

```json
{
  "env": {
    "browser": true,
    "es2021": true
  },
  "extends": [
    "eslint:recommended",
    "plugin:react/recommended",
    "plugin:react-hooks/recommended"
  ],
  "parserOptions": {
    "ecmaFeatures": {
      "jsx": true
    },
    "ecmaVersion": 12,
    "sourceType": "module"
  },
  "plugins": ["react", "react-hooks"],
  "rules": {
    "react/jsx-uses-react": "error",
    "react/jsx-uses-vars": "error",
    "react-hooks/rules-of-hooks": "error",
    "react-hooks/exhaustive-deps": "warn"
  }
}
```
