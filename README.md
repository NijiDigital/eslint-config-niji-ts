## ESLint config rules for TypeScript by Niji

This module provides an ESLint configuration ready to use in any TypeScript project, with enforced rules.

### Installation

with npm:

```shell
npm i -D eslint-config-niji-ts
```

with yarn:

```shell
yarn add -D eslint-config-niji-ts
```

### Getting started

In your `.eslintrc.json`, simply extend the Niji ESLint config:

```json
{
  "$schema": "https://json.schemastore.org/eslintrc.json",
  "env": {
    "es2021": true,
    "node": true
  },
  "extends": ["niji-ts"],
  "parser": "@typescript-eslint/parser",
  "parserOptions": {
    "createDefaultProgram": true,
    "ecmaVersion": 12,
    "project": ["./tsconfig.eslint.json"],
    "sourceType": "module",
    "tsconfigRootDir": "."
  },
  "root": true
}
```

### Enabled rules

All ESLint rules are based on the following dependencies:

- eslint:recommended
- @typescript-eslint/eslint-recommended
- @typescript-eslint/recommended-requiring-type-checking
- @typescript-eslint/recommended-type-checked
- @typescript-eslint/stylistic-type-checked
- prettier/recommended
- sonarjs/recommended
- unicorn/recommended

List of the enabled custom rules:

- @typescript-eslint/adjacent-overload-signatures
- @typescript-eslint/array-type
- @typescript-eslint/ban-tslint-comment
- @typescript-eslint/class-literal-property-style
- @typescript-eslint/consistent-generic-constructors
- @typescript-eslint/consistent-indexed-object-style
- @typescript-eslint/consistent-type-assertions
- @typescript-eslint/consistent-type-definitions
- @typescript-eslint/consistent-type-exports
- @typescript-eslint/consistent-type-imports
- @typescript-eslint/explicit-function-return-type
- @typescript-eslint/explicit-module-boundary-types
- @typescript-eslint/member-ordering
- @typescript-eslint/method-signature-style
- @typescript-eslint/naming-convention
- @typescript-eslint/no-confusing-non-null-assertion
- @typescript-eslint/no-confusing-void-expression
- @typescript-eslint/no-duplicate-enum-values
- @typescript-eslint/no-dynamic-delete
- @typescript-eslint/no-empty-interface
- @typescript-eslint/no-extraneous-class
- @typescript-eslint/no-import-type-side-effects
- @typescript-eslint/no-inferrable-types
- @typescript-eslint/no-invalid-void-type
- @typescript-eslint/no-meaningless-void-operator
- @typescript-eslint/no-mixed-enums
- @typescript-eslint/no-non-null-asserted-nullish-coalescing
- @typescript-eslint/no-require-imports
- @typescript-eslint/no-unnecessary-boolean-literal-compare
- @typescript-eslint/no-unnecessary-condition
- @typescript-eslint/no-unnecessary-qualifier
- @typescript-eslint/no-unnecessary-type-arguments
- @typescript-eslint/no-unsafe-call
- @typescript-eslint/no-useless-empty-export
- @typescript-eslint/non-nullable-type-assertion-style
- @typescript-eslint/parameter-properties
- @typescript-eslint/prefer-enum-initializers
- @typescript-eslint/prefer-for-of
- @typescript-eslint/prefer-function-type
- @typescript-eslint/prefer-includes
- @typescript-eslint/prefer-literal-enum-member
- @typescript-eslint/prefer-namespace-keyword
- @typescript-eslint/prefer-nullish-coalescing
- @typescript-eslint/prefer-optional-chain
- @typescript-eslint/prefer-readonly
- @typescript-eslint/prefer-reduce-type-parameter
- @typescript-eslint/prefer-regexp-exec
- @typescript-eslint/prefer-return-this-type
- @typescript-eslint/prefer-string-starts-ends-with
- @typescript-eslint/prefer-ts-expect-error
- @typescript-eslint/require-array-sort-compare
- @typescript-eslint/sort-type-constituents
- @typescript-eslint/switch-exhaustiveness-check
- @typescript-eslint/typedef
- @typescript-eslint/unified-signatures
- linebreak-style
- no-template-curly-in-string
- prefer-template
- require-await
- simple-import-sort/exports
- simple-import-sort/imports
- sonarjs/elseif-without-else
- sonarjs/no-inverted-boolean-check
- sort-keys-shorthand/sort-keys-shorthand

List of the disabled custom rules:

- @typescript-eslint/explicit-member-accessibility
- @typescript-eslint/no-var-requires
- @typescript-eslint/prefer-readonly-parameter-types
- @typescript-eslint/promise-function-async
- @typescript-eslint/strict-boolean-expressions
- unicorn/filename-case
- unicorn/no-array-reduce
- unicorn/prefer-module
- unicorn/prevent-abbreviations

All these rules are proposed to reach a maximum level of quality without compromise efficiency.

Feel free to customize your configuration to match your needs.

Enjoy!

## [License](https://github.com/NijiDigital/eslint-ts-niji/blob/main/LICENSE)
