# Zak Dental Interactive Call Flow

An interactive web application designed to guide call center agents through standardized call procedures step-by-step.

## Features

### 🎯 **Step-by-Step Navigation**
- **One Step at a Time**: Display only the current step to minimize reading while listening to patients
- **Progress Tracking**: Visual progress bar showing completion status
- **Branch Logic**: Smart navigation based on call scenarios
- **Jump Navigation**: Quick access to any step via dropdown

### 🔍 **Dual Search System**
- **Text Search**: Type keywords to find relevant steps instantly
- **Voice Search**: Use microphone to search hands-free
- **Smart Keywords**: Optimized search terms for call center terminology
- **Search History**: Quick access to recent searches

### 🎙️ **Voice Commands**
- "Next step" - Navigate to next step
- "Previous step" - Go back one step
- "Go to step [number]" - Jump to specific step
- "Bookmark this" - Save current step as bookmark
- "Search [keyword]" - Find steps containing keyword

### 📊 **Agent Helper Features**
- **Call Timer**: Track call duration automatically
- **Agent Notes**: Add personal notes to each step
- **Bookmarks**: Save frequently used steps
- **Quick Actions**: One-click access to common searches

### 🎨 **Customization**
- **5 Themes**: Light, Dark, Blue, Professional, High-contrast
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Accessibility**: WCAG 2.1 compliant with keyboard navigation
- **Agent Personalization**: Save agent name and preferences

## Call Flow Structure

The application breaks down the Zak Dental call flow into 22 organized steps:

### A. **Greeting & Initial Setup** (Steps 1-4)
1. Basic Greeting (Inbound vs Callback)
2. Get Caller Information
3. Confirm Location
4. Ready to Schedule Check

### B. **Specialty Referral Check** (Steps 5-8)
5. Verify Specialty Referral
6. Insurance Verification for Specialty
7. In-Network/Out-of-Network Handling
8. Referral Documentation

### C. **Appointment Type** (Steps 9-11)
9. Single vs Multiple Family Members
10. Insurance Status Check
11. No Insurance Pathway

### D. **Patient Information Gathering** (Steps 12-16)
12. Age-Based Insurance (Medicare vs Dental)
13. Personal Information Collection
14. Insurance Details Entry
15. Referral Source
16. Chart Creation in Denticon

### E. **Appointment Confirmation** (Steps 17-20)
17. Appointment Recap (3+ days)
18. Appointment Recap (<3 days)
19. Special Instructions (Pregnancy, etc.)
20. Final Documentation

### F. **Call Wrap-up** (Steps 21-22)
21. Additional Help Offer
22. Survey Request & Call End

## Quick Start

1. **Open the Application**
   ```
   Open index.html in a web browser
   ```

2. **Enter Your Name**
   - Type your name in the agent field (top left)
   - This will automatically populate in step scripts

3. **Start Your Call**
   - Begin with Step 1 (Basic Greeting)
   - Follow the on-screen instructions
   - Use arrow buttons or keyboard shortcuts to navigate

4. **Use Search When Needed**
   - Type keywords in the search bar
   - Click microphone for voice search
   - Use quick action buttons for common searches

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + ←/→` | Previous/Next step |
| `Ctrl + Home/End` | First/Last step |
| `Ctrl + B` | Bookmark current step |
| `Ctrl + F` | Focus search bar |
| `Ctrl + G` | Jump to step dropdown |
| `Ctrl + Shift + V` | Toggle voice search |
| `Ctrl + Shift + T` | Toggle call timer |
| `F1` or `Ctrl + ?` | Show help dialog |
| `Escape` | Close modals |

## Search Keywords

The app recognizes these key terms:

- **Insurance**: insurance, medicare, benefits, carrier, in-network
- **Scheduling**: schedule, appointment, booking, available
- **Specialty**: specialty, referral, endodontics, oral surgery
- **Location**: location, office, address, convenient
- **Family**: family, multiple, children, names
- **Wrap-up**: wrap up, survey, additional help, end call

## Technical Details

### Browser Compatibility
- **Chrome/Edge**: Full functionality including voice search
- **Firefox**: Full functionality including voice search
- **Safari**: Full functionality including voice search
- **Mobile Browsers**: Responsive design with touch support

### Storage
- All data stored locally in browser
- No server required
- Automatic backup of notes and bookmarks
- Export/import functionality available

### Performance
- Lightweight design (~2MB total)
- Fast loading and navigation
- Optimized for call center environment
- Works offline after initial load

## File Structure

```
call-flow-app/
├── index.html              # Main application file
├── src/
│   ├── components/         # JavaScript components
│   │   ├── StepDisplay.js     # Step content management
│   │   ├── SearchBar.js       # Text search functionality
│   │   ├── VoiceSearch.js     # Voice search & commands
│   │   ├── Navigation.js      # Navigation & bookmarks
│   │   └── ProgressIndicator.js # Progress & timer
│   ├── data/              # Application data
│   │   ├── callFlowSteps.js   # All call flow steps
│   │   └── searchKeywords.js  # Search configuration
│   ├── styles/            # CSS stylesheets
│   │   ├── main.css          # Core styles
│   │   └── themes.css        # Theme definitions
│   └── app.js             # Main application controller
└── README.md              # This file
```

## Deployment

1. **Local Development**:
   - Open `index.html` directly in browser
   - No server setup required

2. **Web Server Deployment**:
   - Upload entire folder to web server
   - No backend requirements
   - Works with any static hosting service

3. **Intranet Deployment**:
   - Deploy to company intranet
   - Accessible via company network
   - Can be bookmarked by agents

## Support & Training

### For Agents
- Press `F1` for built-in help
- Use the microphone icon for hands-free operation
- Bookmark frequently used steps
- Add personal notes to customize your experience

### For Administrators
- No maintenance required
- All data stored locally per agent
- Export functionality for backup
- Customizable themes and content

## Version History

- **v1.0.0** - Initial release with full call flow integration
- Comprehensive step-by-step navigation
- Dual search system (text + voice)
- Agent personalization features
- Multi-theme support
- Complete keyboard accessibility

---

**Contact**: For questions or support, please contact your IT administrator or call center supervisor.