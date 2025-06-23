# One Time Secret - Password.link Extension

A Raycast extension for creating and managing encrypted secrets using [password.link](https://password.link).

## Features

- 🔐 **Create Encrypted Secrets** - Create secure, one-time view secrets with client-side encryption
- 📋 **List & Manage Secrets** - View all your secrets with search and management capabilities
- 🔗 **Secret Requests** - Create request links for collecting secrets from others
- 🗑️ **Delete Secrets** - Remove secrets and secret requests when no longer needed
- 🔧 **Custom Domains** - Support for whitelabel password.link domains
- ⚡ **Fast & Secure** - Built with TypeScript and proper error handling

## Setup

### 1. Get API Keys

1. Sign up for a [password.link](https://password.link) account
2. Navigate to your account settings
3. Generate both a **Public API Key** and **Private API Key**
4. Note your custom domain if you have one (optional)

### 2. Configure Extension

1. Open Raycast and go to Extensions
2. Find "One Time Secret" and click the gear icon
3. Enter your configuration:
   - **Public API Key**: Your password.link public API key
   - **Private API Key**: Your password.link private API key
   - **Base URL**: Your password.link domain (default: https://password.link)

### 3. Start Using

The extension provides four main commands:

- **New Secret**: Create encrypted secrets with various options
- **List Secrets**: View and manage existing secrets
- **New Secret Request**: Create request links for collecting secrets
- **List Secret Requests**: Manage your secret request links

## Commands

### New Secret

Create a new encrypted secret with options for:

- Secret content (required)
- Description and message
- Expiration time (0-350 hours)
- View button (show button instead of auto-display)
- CAPTCHA protection
- Password protection
- Maximum view count (1-100)

### List Secrets

View all your secrets with:

- Search functionality
- Secret status (active/expired)
- View count and creation date
- Quick actions to open or copy URLs
- Delete functionality

### New Secret Request

Create request links for collecting secrets with:

- Description and message
- Expiration and usage limits
- Email notifications
- Default settings for created secrets

### List Secret Requests

Manage your secret request links with:

- Search functionality
- Usage limits and expiration
- Quick actions to open or copy URLs
- Delete functionality

## Security

- All secrets are encrypted client-side before being sent to the server
- API keys are stored securely in Raycast preferences
- Secrets are automatically deleted after being viewed (one-time use)
- Support for additional security features like CAPTCHA and passwords

## Custom Domains

If you have a whitelabel password.link domain, simply enter it in the Base URL preference field. The extension will use your custom domain for all API calls and generated URLs.

## Development

This extension is built with:

- TypeScript for type safety
- React for the UI components
- Raycast API for native integration
- DRY coding principles and early returns
- Comprehensive error handling

## Contributing

Feel free to submit issues and enhancement requests!

## License

MIT License - see LICENSE file for details.
