# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 0.1.x   | :white_check_mark: |

## Reporting a Vulnerability

We take the security of DevLedger seriously. If you believe you have found a security vulnerability, please report it to us as described below.

### Reporting Process

1. **DO NOT** create a public GitHub issue for the vulnerability.
2. Send a description of the vulnerability to [INSERT SECURITY EMAIL].
3. Include as much information as possible:
   - A description of the vulnerability
   - Steps to reproduce the issue
   - Potential impact of the vulnerability
   - Any potential solutions you've identified

### What to Expect

- We will acknowledge receipt of your vulnerability report within 48 hours.
- We will send you regular updates about our progress.
- If you have followed the instructions above, we will not take any legal action against you regarding your report.

## Security Considerations

DevLedger handles sensitive information through:
- Code comments and technical documentation
- API keys for LLM services
- Local and cloud model configurations
- Git repository data

### Security Features

1. **API Key Management**
   - Secure storage in `.env` files (gitignored)
   - Environment variable support
   - Configurable key rotation policies

2. **Local Model Support**
   - Option to use local LLMs for sensitive environments
   - No data transmission to external services when using local models

3. **Data Privacy**
   - Configurable privacy settings for comment processing
   - Local-first architecture
   - Optional cloud features

4. **Access Control**
   - Repository-level access controls through Git
   - Configurable visibility settings for `.devl` files

## Best Practices

When using DevLedger:
1. Always use `.env` files or environment variables for API keys
2. Regularly review and update access permissions
3. Use local models when processing sensitive information
4. Keep the software updated to the latest supported version
5. Follow security guidelines in the documentation

## Security Updates

Security updates will be released as patch versions. We recommend always using the latest version of DevLedger to ensure you have all security patches.

## Acknowledgments

We would like to thank the following for their contributions to DevLedger's security:
- Security researchers who responsibly disclose vulnerabilities
- The open source community for security-related improvements