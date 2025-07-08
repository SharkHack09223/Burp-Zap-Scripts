# Burp Suite & OWASP ZAP Security Scripts Repository

A comprehensive collection of custom scripts and extensions for Burp Suite and OWASP ZAP to enhance web application security testing capabilities.

## 📋 Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Scripts Collection](#scripts-collection)
- [Usage Examples](#usage-examples)
- [Script Categories](#script-categories)
- [Contributing](#contributing)
- [Prerequisites](#prerequisites)
- [License](#license)
- [Disclaimer](#disclaimer)

## 🔍 Overview

This repository contains a curated collection of security testing scripts designed for:
- **Burp Suite Professional/Community** - Extensions and plugins
- **OWASP ZAP** - Active/Passive scan rules and scripts
- **Security Testing** - Automated vulnerability detection and analysis

### Key Features

- ✅ **Comprehensive Coverage** - SQL Injection, XSS, Authentication, Authorization
- ✅ **Ready-to-Use** - No complex setup required
- ✅ **Well-Documented** - Clear instructions and examples
- ✅ **Actively Maintained** - Regular updates and improvements
- ✅ **Educational** - Learn from real-world security testing scenarios

## 🚀 Installation

### Burp Suite Extensions

1. **Via Burp Suite GUI:**
   ```
   Extensions → Burp App Store → Load Extension
   ```

2. **Manual Installation:**
   ```bash
   # Clone repository
   git clone https://github.com/your-username/burp-zap-scripts.git
   
   # Navigate to Burp Suite
   Extensions → Extensions → Add → Select Python file
   ```

### OWASP ZAP Scripts

1. **Via ZAP GUI:**
   ```
   Tools → Options → Scripts → Load Script
   ```

2. **Script Directory:**
   ```bash
   # Copy scripts to ZAP scripts directory
   cp zap-scripts/* ~/.ZAP/scripts/
   ```

## 📁 Scripts Collection

### Burp Suite Extensions

| Script | Category | Description | Status |
|--------|----------|-------------|--------|
| `jwt_extractor.py` | Authentication | Extract and decode JWT tokens | ✅ Active |
| `custom_header_injector.py` | Headers | Inject custom headers for testing | ✅ Active |
| `cookie_analyzer.py` | Session Management | Analyze cookie security attributes | 🔄 In Progress |
| `csrf_detector.py` | CSRF | Detect CSRF vulnerabilities | 📋 Planned |
| `cors_scanner.py` | CORS | Test CORS misconfigurations | 📋 Planned |

### OWASP ZAP Scripts

| Script | Type | Category | Description | Status |
|--------|------|----------|-------------|--------|
| `sql_injection_scanner.py` | Active | Injection | Advanced SQL injection detection | ✅ Active |
| `xss_scanner.py` | Active | Injection | Comprehensive XSS vulnerability scanner | ✅ Active |
| `lfi_scanner.py` | Active | Injection | Local File Inclusion detector | 🔄 In Progress |
| `sensitive_data_exposure.py` | Passive | Information Disclosure | Detect sensitive data in responses | 📋 Planned |
| `security_headers_check.py` | Passive | Configuration | Check security headers | 📋 Planned |

## 💡 Usage Examples

### JWT Token Extractor (Burp Suite)

```python
# Automatically extracts JWT tokens from HTTP traffic
# View extracted tokens in dedicated tab
# Decodes header and payload for analysis
```

**Features:**
- Real-time JWT extraction
- Base64 decoding
- JSON formatting
- Token validation

### SQL Injection Scanner (ZAP)

```python
# Comprehensive SQL injection testing
# Multiple payload types and databases
# Error-based, time-based, and boolean-based detection
```

**Payload Types:**
- MySQL, PostgreSQL, Oracle, SQL Server
- Union-based injections
- Time-based blind SQL injection
- Error-based detection

### Custom Header Injector (Burp Suite)

```python
# Inject custom headers for bypass testing
# Predefined security headers
# Export/import functionality
```

**Common Headers:**
- `X-Forwarded-For`
- `X-Real-IP`
- `X-HTTP-Method-Override`
- `Authorization`

## 🏷️ Script Categories

### 🔒 Authentication & Authorization
- JWT token analysis
- Session management testing
- OAuth vulnerabilities
- Multi-factor authentication bypass

### 💉 Injection Vulnerabilities
- SQL injection detection
- XSS (Cross-Site Scripting)
- Command injection
- LDAP injection
- NoSQL injection

### 🌐 Web Application Security
- CORS misconfiguration
- CSRF protection bypass
- Security headers analysis
- File upload vulnerabilities

### 📊 Information Disclosure
- Sensitive data exposure
- Debug information leakage
- Error message analysis
- Directory traversal

### ⚙️ Configuration & Deployment
- Security headers validation
- SSL/TLS configuration
- Server information disclosure
- HTTP methods testing

## 🛠️ Prerequisites

### Burp Suite Requirements
- **Burp Suite Professional/Community** (Latest version recommended)
- **Jython 2.7+** (for Python extensions)
- **Java 8+**

### OWASP ZAP Requirements
- **OWASP ZAP 2.10+**
- **Python 3.6+**
- **Jython 2.7+** (for Python scripts)

### Development Environment
```bash
# Python dependencies
pip install requests beautifulsoup4 urllib3

# Java dependencies (if applicable)
# Add to classpath as needed
```

## 🤝 Contributing

We welcome contributions! Please follow these guidelines:

### How to Contribute

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/new-script
   ```
3. **Add your script with documentation**
4. **Test thoroughly**
5. **Submit a pull request**

### Contribution Guidelines

- ✅ Follow existing code structure
- ✅ Include comprehensive documentation
- ✅ Add usage examples
- ✅ Test with multiple scenarios
- ✅ Follow security best practices

### Script Requirements

- **Header comment** with description and usage
- **Error handling** for robust execution
- **User-friendly interface** (if applicable)
- **Performance optimization**
- **Security considerations**

## 📖 Documentation

### Script Documentation Template

```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-
"""
Script Name - Tool Type (Burp Suite/ZAP)
Brief description of functionality

Author: Your Name
Version: 1.0
Date: YYYY-MM-DD
License: MIT

Usage:
    Detailed usage instructions

Features:
    - Feature 1
    - Feature 2

Requirements:
    - Requirement 1
    - Requirement 2
"""
```

## 🔐 Security Considerations

### Important Notes

⚠️ **Warning:** These scripts are for authorized security testing only

- Only use on systems you own or have explicit permission to test
- Some scripts may generate significant traffic
- Always follow responsible disclosure practices
- Consider impact on production systems

### Best Practices

- Test in isolated environments first
- Monitor resource usage
- Implement rate limiting where appropriate
- Log activities for audit trails

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### MIT License Summary
- ✅ Commercial use
- ✅ Modification
- ✅ Distribution
- ✅ Private use
- ❌ Liability
- ❌ Warranty

## ⚠️ Disclaimer

This repository is intended for educational and authorized security testing purposes only. Users are responsible for ensuring they have proper authorization before using these scripts on any systems. The authors are not responsible for any misuse or damage caused by these tools.

## 🆘 Support

### Getting Help

- **Issues:** Report bugs or request features via GitHub Issues
- **Discussions:** Join community discussions
- **Documentation:** Check individual script documentation
- **Examples:** Review usage examples in `/examples` directory

### Contact

- **GitHub:** [@your-username](https://github.com/your-username)
- **Email:** your.email@example.com
- **Twitter:** [@your-handle](https://twitter.com/your-handle)

## 📊 Statistics

![GitHub stars](https://img.shields.io/github/stars/your-username/burp-zap-scripts)
![GitHub forks](https://img.shields.io/github/forks/your-username/burp-zap-scripts)
![GitHub issues](https://img.shields.io/github/issues/your-username/burp-zap-scripts)
![GitHub license](https://img.shields.io/github/license/your-username/burp-zap-scripts)

## 🎯 Roadmap

### Upcoming Features

- [ ] **GUI Enhancement** - Improved user interfaces
- [ ] **API Integration** - External tool integration
- [ ] **Machine Learning** - AI-powered vulnerability detection
- [ ] **Reporting** - Enhanced reporting capabilities
- [ ] **Cloud Integration** - Cloud security testing scripts

### Version History

- **v1.0.0** - Initial release with basic scripts
- **v1.1.0** - Added JWT extractor and SQL injection scanner
- **v1.2.0** - Enhanced XSS detection and header injection
- **v2.0.0** - Major refactoring and new features (planned)

---

**⭐ If you find this repository useful, please give it a star!**

**🔗 Share with the security community to help others learn and improve their testing capabilities.**







