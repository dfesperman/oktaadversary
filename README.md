# Security Training: Phishing Attack Demonstration

## 🎓 Educational Purpose

This application is a **security awareness training tool** designed to demonstrate how phishing attacks work and how threat actors harvest credentials. It shows both sides of a phishing attack:

1. **User Side**: A convincing fake login page (modeled after Okta)
2. **Attacker Side**: An admin panel showing how credentials are captured in real-time

## ⚠️ Important Disclaimer

**THIS IS FOR EDUCATIONAL AND TRAINING PURPOSES ONLY**

- Never use this tool for malicious purposes
- Only use with explicit permission in controlled training environments
- Do not enter real credentials into the demonstration
- All captured data is stored locally in browser localStorage

## 📋 Features

### Phishing Demo Page (index.html)
- Realistic Okta-style login interface
- Captures username, password, and other form data
- Clear educational warnings
- Simulates credential harvesting
- Visual success feedback when credentials are "captured"

### Admin Panel (admin.html)
- Real-time dashboard showing captured credentials
- Statistics: Total captures, today's captures, last capture time
- Live auto-refresh option (5-second intervals)
- Export captured data to CSV
- Clear all captured data
- Responsive design for any screen size

## 🚀 How to Use

1. **Open the Phishing Demo**
   - Open `index.html` in a web browser
   - This represents what a victim would see

2. **Enter Test Credentials**
   - Use fake credentials only (e.g., "testuser", "password123")
   - Click "Sign In"
   - Credentials are captured and stored locally

3. **View Admin Panel**
   - Click the "View Admin Panel" button or open `admin.html`
   - See all captured credentials displayed in a table
   - Enable auto-refresh to see real-time updates

4. **Export or Clear Data**
   - Use the "Export CSV" button to download captured data
   - Use "Clear All" to reset the demonstration

## 🛡️ Security Training Use Cases

### What This Demonstrates

1. **Visual Deception**: How attackers create convincing fake login pages
2. **Credential Harvesting**: How user input is captured and stored
3. **Data Exfiltration**: How stolen credentials are collected and exported
4. **Attack Monitoring**: How attackers monitor their phishing campaigns

### Training Points

- **Always verify the URL** before entering credentials
- **Look for HTTPS** and valid certificates
- **Be suspicious of unexpected login pages**
- **Use password managers** that auto-fill only on legitimate sites
- **Enable multi-factor authentication** (MFA)
- **Report suspicious sites** to IT security

## 📊 Technical Details

### Technology Stack
- Pure HTML, CSS, and JavaScript
- No backend server required
- Uses browser localStorage for data persistence
- Responsive design with modern CSS

### Data Storage
- All data stored in browser localStorage
- Data persists until manually cleared
- Each browser/device has its own isolated storage
- No data leaves the local machine

### Browser Compatibility
- Works in all modern browsers (Chrome, Firefox, Safari, Edge)
- Requires JavaScript enabled
- Responsive design for mobile and desktop

## 🎯 Training Scenarios

### Scenario 1: Basic Phishing Recognition
1. Show participants the phishing page
2. Ask them to identify red flags
3. Discuss the warning banners and URL verification

### Scenario 2: Credential Capture Demonstration
1. Enter test credentials on the phishing page
2. Switch to admin panel to show real-time capture
3. Discuss how attackers monitor campaigns

### Scenario 3: Defense Strategies
1. Demonstrate how password managers detect fake sites
2. Show the importance of MFA
3. Discuss reporting procedures

## 📝 Customization

You can customize the phishing page to match different services:
- Change colors and branding in the CSS
- Modify the logo and text
- Add or remove form fields
- Adjust the warning banners

## 🔒 Best Practices

When using this training tool:

1. **Clear Communication**: Always inform participants this is a training exercise
2. **Controlled Environment**: Use only in designated training sessions
3. **No Real Credentials**: Emphasize using test data only
4. **Document Usage**: Keep records of training sessions
5. **Clean Up**: Clear captured data after each session
6. **Follow-up**: Provide actionable security guidance

## 📚 Additional Resources

- NIST Phishing Guidance: https://www.nist.gov/itl/applied-cybersecurity/tig/back-basics-multi-factor-authentication
- CISA Phishing Resources: https://www.cisa.gov/news-events/news/avoiding-social-engineering-and-phishing-attacks
- Security Awareness Training: https://www.sans.org/security-awareness-training/

## 🤝 Support

For questions or issues with this training tool, contact your security team or training coordinator.

---

**Remember: The best defense against phishing is education and awareness!** 🛡️
