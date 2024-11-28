# Contributing to MCP Documentation

Thank you for your interest in contributing to the Model Context Protocol (MCP) documentation! This guide will help you get started with contributing.

## Getting Started

1. Install the required tools:
   - Node.js
   - Git
   - [Mintlify CLI](https://www.npmjs.com/package/mintlify): `npm i -g mintlify`
2. Fork and clone the repository
3. Create a new branch for your changes
4. Run `mintlify dev` to preview changes locally

## Signing Your Commits

We require all commits to be signed to verify the identity of contributors. Here's how to set up commit signing:

1. Generate a GPG key if you don't have one:

   ```bash
   gpg --full-generate-key
   ```

   - Choose RSA and RSA (default)
   - Choose 4096 bits
   - Enter your name and email (must match GitHub email)

2. Get your GPG key ID:

   ```bash
   gpg --list-secret-keys --keyid-format=long
   ```

3. Configure Git to use your GPG key:

   ```bash
   git config --global user.signingkey YOUR_KEY_ID
   git config --global commit.gpgsign true
   ```

4. Add your GPG key to GitHub:

   - Copy your GPG key: `gpg --armor --export YOUR_KEY_ID`
   - Go to GitHub Settings > SSH and GPG keys
   - Click "New GPG key" and paste your key

5. For each commit, use:
   ```bash
   git commit -S -m "Your commit message"
   ```
   The `-S` flag signs your commit. With `commit.gpgsign` configured, you can omit the `-S` flag.

Note: On Windows, you might need to [download GPG4Win](https://www.gpg4win.org/) and configure its path in Git.

[You can learn more about signed commits here.](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification)

## Documentation Guidelines

- Keep content clear, concise, and technically accurate
- Follow the existing file structure and naming conventions
- Include code examples where appropriate
- Use proper MDX formatting and components
- Test all links and code samples

## Content Types

You can contribute to:

- Conceptual guides
- API reference documentation
- Tutorials and quickstarts
- Best practices and examples
- Troubleshooting guides

## Pull Request Process

1. Ensure your changes follow our documentation guidelines
2. Update the relevant table of contents if needed
3. Test your changes locally using `mintlify dev`
4. Submit a pull request with a clear description of your changes
5. Wait for review and address any feedback

## Need Help?

- Check existing documentation at [modelcontextprotocol.io](https://modelcontextprotocol.io)
- [Open an issue](https://github.com/modelcontextprotocol/docs/issues) for bugs or concerns
- Join our [community discussions](https://github.com/modelcontextprotocol/docs/discussions)

## Code of Conduct

Please note that this project follows our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you agree to uphold these guidelines.
