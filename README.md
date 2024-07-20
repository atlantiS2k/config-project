Custom Configuration
This project includes my custom configuration that I use across all my projects. Here's a brief overview of the setup:

ESLint
The project uses ESLint to maintain code quality and consistency. The configuration includes:

Base Configuration: Extends eslint:recommended and plugin:@typescript-eslint/recommended.
Prettier Integration: Ensures that code formatting follows Prettier rules.
Plugins: Includes @typescript-eslint, unused-imports, simple-import-sort, and prettier.
Rules: Custom rules for linting, including naming conventions, sorting imports, and handling unused imports.
Prettier
Prettier is used for code formatting. The configuration includes:

Semi: Requires semicolons at the end of statements.
Trailing Comma: Includes trailing commas where valid in ES5 (e.g., objects, arrays).
Single Quote: Uses single quotes for strings.
Print Width: Wraps lines at 80 characters.
Tab Width: Uses 2 spaces for indentation.
Use Tabs: Disables tab characters; uses spaces instead.
Bracket Spacing: Adds spaces between brackets in object literals.
Arrow Parens: Avoids parentheses around a sole arrow function parameter.
End Of Line: Uses LF for line endings.
Husky
Husky is used to enforce commit message conventions and run pre-commit hooks. The configuration includes:

Commit Message Hook: Ensures that commit messages follow the format type: description, where type can be bugfix, release, feat, config, or chore.
Pre-commit Hook: Runs lint-staged to lint and format code before commits.
lint-staged
lint-staged is used to run linters and formatters on pre-committed files. The configuration includes:

JavaScript and TypeScript Files: Runs ESLint and Prettier on JavaScript and TypeScript files.
SCSS Files: Runs Prettier on SCSS files.
