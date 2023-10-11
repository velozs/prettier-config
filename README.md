
# @velozs/prettier-config

This package provides a Prettier configuration file that you can use in your projects to maintain consistent code formatting. Prettier is an opinionated code formatter that enforces a consistent coding style across your codebase.

## Configuration

The Prettier configuration in this package is defined in a `index.json` file, and it enforces the following formatting rules:

```json
{
  "trailingComma": "es5",
  "tabWidth": 2,
  "semi": true,
  "singleQuote": true,
  "printWidth": 80
}
```

You can adjust these settings to match your project's coding style preferences. Here's a brief explanation of each configuration option:

- `trailingComma`: This option controls the usage of trailing commas in object literals. In this configuration, it's set to `"es5"`, which means it uses a trailing comma whenever valid in an ES5 environment.

- `tabWidth`: The number of spaces Prettier uses for each level of indentation.

- `semi`: Determines whether to add semicolons at the end of statements.

- `singleQuote`: Specifies whether to use single quotes for strings.

- `printWidth`: Sets the maximum line length for formatting.

## Usage

To use this Prettier configuration in your project, follow these steps:

1. Install Prettier as a development dependency if you haven't already:

   ```bash
   npm install --save-dev prettier
   # or
   yarn add --dev prettier
   ```

2. Create a `.prettierrc` file or add the configuration directly to your `package.json`:

   **Option 1: Create a `.prettierrc` file**

   Create a `.prettierrc` file in the root of your project and add the following content:

   ```json
   {
     "extends": "@velozs/prettier-config"
   }
   ```

   **Option 2: Add the configuration to your `package.json`**

   You can also include the configuration directly in your `package.json` file:

   ```json
   {
     "prettier": "@velozs/prettier-config"
   }
   ```

3. That's it! Now Prettier will format your code according to the configuration in this package.

## Contributing

If you have suggestions, improvements, or want to report issues related to this Prettier configuration, please feel free to open an issue or submit a pull request in the [GitHub repository](https://github.com/yourusername/my-awesome-prettier-config).

## License

This Prettier configuration is open-source and available under the [MIT License](LICENSE). Feel free to use and modify it for your projects.

Happy coding!
