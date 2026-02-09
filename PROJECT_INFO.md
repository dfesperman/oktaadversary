# OktaAdversary - Identity Attack Training Platform

A comprehensive security awareness training application demonstrating various identity-related attacks.

## 🎯 Project Overview

**OktaAdversary** is an educational tool designed to help security professionals and organizations understand how threat actors execute identity-based attacks. The platform provides realistic simulations of common attack vectors in a safe, controlled environment.

### Current Version: 1.0.0

## 📁 Project Structure

```
phishing-training/
├── index.html          # Phishing demo page (user-facing)
├── admin.html          # Admin monitoring panel (attacker's view)
├── icon.png            # Spider icon for branding
├── README.md           # User documentation
├── PROJECT_INFO.md     # This file - project information
└── .gitignore          # Git ignore rules
```

## 🚀 Features

### Current Features (v1.0)

#### Adversary-in-the-Middle Attack Simulation
- **Phishing Demo Page**:
  - Authentic Okta-style login interface
  - Configurable to mimic any target URL
  - Real-time credential capture
  - Mobile-responsive design
  - Educational warning banner

- **Admin Monitoring Panel**:
  - Beautiful dark-mode dashboard
  - Real-time credential monitoring
  - Statistics and analytics
  - Auto-refresh capability
  - CSV export functionality
  - Tab-based navigation for multiple attack types

### Planned Features (Coming Soon)
- 🔑 **Credential Stuffing & Password Spraying**
- 📱 **MFA Fatigue Attack**
- 🔓 **Session Hijacking**

## 💻 Technology Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript
- **Storage**: Browser localStorage
- **Dependencies**: None (fully self-contained)
- **Server**: Not required (static files only)

## 🛠️ Installation & Setup

### Option 1: Local Use (Simple)
1. Download/clone this repository
2. Open `index.html` in any modern web browser
3. Access the admin panel via the green button or open `admin.html` directly

### Option 2: Web Server (Recommended for Training)
```bash
# Using Python 3
cd phishing-training
python3 -m http.server 8000

# Using Node.js (with npx)
npx http-server -p 8000

# Access at: http://localhost:8000
```

### Option 3: Deploy to Web Server
Upload all files to any web server (Apache, Nginx, etc.) and access via your domain.

## 📖 Usage

### For Training Sessions

1. **Setup Phase**:
   - Open `admin.html` in one browser tab/window
   - Configure target URL in the admin panel
   - Clear any previous test data

2. **Demonstration Phase**:
   - Show participants the phishing page (`index.html`)
   - Discuss red flags and warning signs
   - Have participants enter test credentials
   - Switch to admin panel to show real-time capture

3. **Discussion Phase**:
   - Review captured data
   - Export to CSV for analysis
   - Discuss defense strategies

### Configuration

The admin panel allows you to configure the phishing page to mimic different target services:
- Enter any URL in the configuration panel
- Click "Update UI"
- The phishing page will adapt its branding

## 🔒 Security & Privacy

### Important Notes
- All data is stored locally in browser localStorage
- No data is transmitted to external servers
- No backend or database required
- Designed for isolated training environments

### Best Practices
- ✅ Use only in controlled training sessions
- ✅ Always use test/fake credentials
- ✅ Clear captured data after each session
- ✅ Inform all participants this is a simulation
- ❌ Never deploy publicly without proper safeguards
- ❌ Never enter real credentials

## 📊 Data Management

### Data Storage
- Credentials stored in: `localStorage.capturedCredentials`
- Target URL config stored in: `localStorage.phishingTargetUrl`

### Data Export
- Use the "Export CSV" button in admin panel
- Format: Timestamp, Username, Password, Remember Me, User Agent, IP

### Data Cleanup
```javascript
// Clear all captured credentials
localStorage.removeItem('capturedCredentials');

// Clear target URL configuration
localStorage.removeItem('phishingTargetUrl');
```

## 🎨 Customization

### Branding
- Edit CSS in `index.html` for phishing page styling
- Edit CSS in `admin.html` for admin panel theme
- Replace `icon.png` with custom icon

### Attack Simulations
The codebase is structured to easily add new attack types:
1. Add new tab in sidebar navigation
2. Create corresponding tab content section
3. Implement attack-specific logic

## 🐛 Known Issues

- localStorage has size limits (~5-10MB depending on browser)
- Auto-refresh may impact performance with many records
- Social login buttons are non-functional (by design)

## 🔄 Version History

### v1.0.0 (Current)
- ✅ Adversary-in-the-Middle (phishing) simulation
- ✅ Admin monitoring dashboard
- ✅ Dark mode UI with gradients
- ✅ Multi-attack type navigation
- ✅ CSV export functionality
- ✅ Configurable target URL
- ✅ Real-time credential capture

## 🤝 Contributing

This project is designed for educational purposes. If you'd like to contribute:
1. Fork the repository
2. Create a feature branch
3. Test thoroughly in isolated environment
4. Submit pull request with detailed description

## 📝 License

This software is provided for educational and training purposes only. Use responsibly and ethically.

## ⚠️ Disclaimer

**FOR EDUCATIONAL USE ONLY**

This tool is designed solely for security awareness training and education. Users must:
- Only use in authorized training environments
- Obtain proper permissions before deployment
- Never use for malicious purposes
- Comply with all applicable laws and regulations

The creators assume no liability for misuse of this software.

## 📧 Support

For questions or issues:
- Review the README.md for usage instructions
- Check the code comments for implementation details
- Contact your security team or training coordinator

## 🙏 Acknowledgments

- Built for security awareness training
- Designed to educate users about identity threats
- Inspired by real-world attack patterns

---

**Built with Claude Code** - Teaching security through simulation 🛡️
