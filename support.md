# CPR Timer - Support & User Guide

## App Overview

CPR Timer is a professional tool designed to assist trained healthcare workers during cardiopulmonary resuscitation (CPR) procedures. The app helps track CPR cycles, manage medication timing, record events, and calculate important metrics like Chest Compression Fraction (CCF).

**MEDICAL DISCLAIMER**: This app is a tool to assist trained medical professionals during CPR. It is NOT a substitute for proper CPR training and certification. It is NOT intended for use by untrained individuals. Always follow your institution's protocols and guidelines. The developers assume no liability for clinical decisions made using this app.

---

## Target Audience

This app is designed for:
- Emergency medicine physicians
- Intensive care unit staff
- Anesthesiologists
- Nurses and paramedics
- Other trained healthcare professionals performing CPR

---

## Getting Started

### First Time Setup

1. Download and install CPR Timer from the App Store
2. Open the app to see the main CPR Tracker interface
3. Choose your preferred mode: **Coach** or **Track**
   - **Coach Mode** (Default): Provides automatic alerts, voice prompts, and medication reminders
   - **Track Mode**: Manual tracking without automatic alerts
4. Optionally sign in to save sessions to the cloud

### Understanding the Interface

The main screen shows:
- **Total CPR Time**: Cumulative time since CPR started
- **Current Cycle**: 2-minute CPR cycles
- **Event Banners**: Pulse check, medications (Adrenaline, Amiodarone, Xylocaine)
- **LUCAS Toggle**: Activate when LUCAS device is in use
- **Rhythm Selector**: Choose between Shockable (VF/VT) or Non-shockable (PEA/Asystole)
- **Statistics**: Shock count, medication counts, and progress bars

---

## Core Features

### Coach Mode vs Track Mode

**Coach Mode** (Green toggle):
- Automatic time-based alerts for medications
- Configurable metronome beeping (100/110/120 BPM)
- Voice alerts for pulse checks and medications (English/Thai)
- Automatic medication reminders based on protocol timings
- Audio feedback for actions

**Track Mode** (Gray toggle):
- Manual medication tracking
- No automatic alerts or sounds
- User must manually confirm or give medications
- Event logging only

**Switching Modes**: Use the toggle switch at the top-right of the Cycle Tracker panel. The app will display a notification when you switch modes.

---

## Starting a CPR Session

1. Tap **"Start CPR"** button
2. The timer begins immediately
3. The app will:
   - Start tracking total CPR time
   - Begin 2-minute cycle countdown
   - Start metronome (if in Coach mode)
   - Activate event banners

### Adding Time Delay

If CPR started before you opened the app:
1. Open the hamburger menu (☰)
2. Tap **"Add Time Delay"**
3. Enter the number of minutes CPR was already in progress
4. Confirm - the timer will adjust retroactively

---

## During a CPR Session

### Cycle Management

- Each cycle lasts **2 minutes**
- The timer shows countdown to next cycle
- Last 10 seconds show amber warning: "PREPARE FOR CYCLE CHANGE"
- After 2 minutes, the cycle number increments automatically

### Rhythm Selection

Choose the cardiac rhythm:

**Shockable (VF/VT)**:
- Enables shock delivery
- Medications available: Adrenaline, Amiodarone, Lidocaine
- Protocol follows shockable rhythm guidelines

**Non-Shockable (PEA/Asystole)**:
- Shock button disabled
- Focus on compressions and medications
- Banner shows: "Continue CPR"

### LUCAS Device

- Toggle LUCAS switch when activating the LUCAS device
- When active, shocks do NOT count toward pause time (CCF calculation)
- LUCAS banner turns blue when active
- Located next to Pulse Check banner

### Delivering Shocks

1. Ensure rhythm is set to "Shockable"
2. Select energy level:
   - **Biphasic**: 200J (adult) or Pediatric options
   - **Monophasic**: 360J
3. Tap **"Shock"** button
4. Shock is logged with timestamp and energy level
5. Shock counter increments

### Medication Administration

#### Adrenaline (1mg)

**In Coach Mode**:
- First dose: Alert after 4 minutes (configurable to 3 or 5 minutes)
- Subsequent doses: Every 4 minutes (or your configured interval)
- Audio alert and voice prompt when due
- Tap **"Confirm"** when given, or **"Dismiss"** to skip

**In Track Mode**:
- Manually tap **"Give"** button when administering
- No automatic alerts

**Configuring Interval**:
1. Open hamburger menu
2. Under "Adrenaline Interval", select 3, 4, or 5 minutes
3. Setting applies to current and future doses

#### Amiodarone

**Protocol**: 300mg first dose, then 150mg second dose (total 450mg)

**In Coach Mode**:
- First dose (300mg): Alert after 3rd shock in shockable rhythm
- Second dose (150mg): Alert after 5th shock
- Voice alert when due

**In Track Mode**:
- Tap **"Give"** when appropriate
- Can manually select dose (300mg or 150mg)

#### Lidocaine/Xylocaine

**Protocol**: Given after Amiodarone 450mg has been reached

**In Coach Mode**:
- First dose (1mg/kg): Alert 5 minutes after amiodarone 450mg
- Subsequent doses: Every 5 minutes
- Maximum 3mg/kg cumulative dose
- Voice alert when due

**In Track Mode**:
- Manually give when appropriate
- Select dose (1mg/kg or 0.5mg/kg)

### Pulse Checks

**Timing**: Every 2-minute cycle

**In Coach Mode**:
- Automatic alert at end of each cycle
- Voice prompt: "Pulse check"
- Tap **"Confirm"** after checking

**In Track Mode**:
- Tap **"Give"** when performing pulse check

### Recording Procedures

During CPR, you can log procedures:
1. Tap **"+ Procedure"** button
2. Select procedure type:
   - Endotracheal Tube (ETT)
   - Arterial Line
   - Central Line
   - Other
3. Procedure is timestamped and logged
4. ETT automatically adds 10 seconds to pause time (affects CCF)

---

## Session Controls (Hamburger Menu)

Access the hamburger menu (☰) for additional controls:

### Session Controls

**Add Time Delay**:
- Add retroactive CPR time if CPR started before app
- Shows total delay added
- Button turns green when delay has been added
- Only available after session started

**Language Toggle (EN/TH)**:
- Switch between English and Thai voice alerts
- Button shows current language
- Blue when Thai selected, gray when English
- Only available after session started

### Metronome Speed

Select compression rate:
- **100 BPM**: Standard rate
- **110 BPM**: Faster compressions
- **120 BPM**: High-performance rate

Purple highlight shows active selection.

### Adrenaline Interval

Configure time between adrenaline doses:
- **3 minutes**: Aggressive protocol
- **4 minutes**: Standard (default)
- **5 minutes**: Conservative

Purple highlight shows active selection.

### Navigation

- **CPR Tracker**: Return to main tracking screen
- **Records**: View saved sessions (disabled during active CPR)

### Authentication

- **Sign In**: Save sessions to cloud, sync across devices
- **Sign Out**: Confirm before signing out

---

## Special Events

### ROSC (Return of Spontaneous Circulation)

When ROSC is achieved:
1. Tap **"ROSC"** button
2. Confirm in dialog
3. All alerts and sounds are suppressed
4. Banners turn green (completed state)
5. ROSC time is recorded
6. Can still end session or continue monitoring

### ECMO Run

When ECMO is initiated:
1. Select rhythm as "PEA" or "Asystole"
2. Open procedure menu
3. Select "ECMO Run"
4. All alerts and sounds are suppressed
5. CPR tracking continues for time calculations

---

## Ending a Session

### Steps to End Session

1. Tap **"End Session"** button
2. Confirm ending the session
3. Fill out the End CPR Session form

### Required Information

**Outcome** (Required):
- **ROSC**: Return of spontaneous circulation achieved
- **Death**: Patient declared deceased
- **ECMO**: Patient placed on ECMO
- **Ongoing/Transfer**: CPR continuing or patient transferred

### Event Timing

The form shows your CPR start time for reference. You can enter times as **duration before CPR started**:

**Collapse Time (Time of Arrest)**:
- Enter hours and minutes before CPR started
- Leave blank if unknown (unwitnessed arrest)
- Example: If arrest was 15 minutes before CPR started, enter "0 hr 15 min"

**Bystander CPR Start Time**:
- Enter when bystander CPR was started (as duration before your CPR)
- Leave blank if no bystander CPR
- Example: If bystander CPR started 10 minutes before your CPR, enter "0 hr 10 min"

**Pause Duration Per Pulse Check**:
- Estimate seconds paused for each pulse check
- Default: **10 seconds**
- Used to calculate Chest Compression Fraction
- Shorter pauses = better CCF
- Range: 0-60 seconds

### Patient Demographics (Optional)

- **Patient Name**: Full name
- **Hospital Number (HN)**: Patient identifier
- **Hospital Name**: Your institution
- **Location**: Ward type (ER, ICU, OR, Ward, etc.)
- **Sex**: Male, Female, Other
- **Age**: Patient age in years

### Session Notes (Optional)

**CPR Session Note**:
- Add any relevant notes about the CPR event
- Clinical observations
- Special circumstances
- Multiple lines supported

### Saving the Session

1. Fill out required outcome
2. Add optional information as needed
3. Tap **"End & Save Session"** (if signed in) or **"End & Sign In to Save"** (if guest)
4. Session is saved with all events, timestamps, and statistics
5. Loading indicator prevents duplicate saves

**Note**: Guest users must sign in to save sessions. The sign-in dialog will appear after tapping save.

---

## Session Records

### Viewing Records

1. Ensure CPR session is ended (cannot access during active session)
2. Tap hamburger menu → **"Records"**
3. View list of all saved sessions

**Sign In Required**: Records are only available for authenticated users.

### Record Information

Each record shows:
- Session date and time
- Total CPR duration
- Outcome
- Patient information (if provided)
- Chest Compression Fraction (CCF)

### Viewing Session Details

Tap a record to view:

**Overview Tab**:
- CPR start/end time
- Outcome
- Collapse time (if recorded)
- Bystander CPR time (if recorded)
- CPR session notes

**Timeline Tab**:
- Chronological list of all events
- Color-coded by type:
  - Blue: Rhythm changes
  - Yellow: Shocks
  - Red: Adrenaline
  - Purple: Amiodarone
  - Teal: Lidocaine
  - Green: Procedures
  - Orange: Bystander CPR

**Statistics Tab**:
- Total CPR time
- Chest Compression Fraction (CCF)
- Number of shocks and energy levels
- Medication counts and timing
- Procedure list

### Exporting Records

1. Open a record
2. Tap **"Export HTML"** button
3. HTML file is generated with complete session data
4. Can be opened in any web browser
5. Suitable for printing or archiving

**Note**: Export contains all session data, timeline, and statistics in a formatted HTML document.

### Data Management

**Collapse Time and Bystander CPR Time**:
- These fields are read-only in record details
- Set during session end form only
- Displayed as "Not recorded" if not entered

**Post CPR Session Notes**:
- Not displayed in record details view
- CPR Session Notes remain visible

---

## Understanding Calculations

### Chest Compression Fraction (CCF)

**What It Measures**:
CCF represents the percentage of CPR time when chest compressions were actually being performed.

**Formula**:
```
CCF = (Total CPR Time - Total Pause Time) / Total CPR Time × 100%
```

**Pause Time Includes**:
- Pulse checks (default 10 seconds each, configurable)
- ETT insertion (10 seconds)
- Shocks (5 seconds each, unless LUCAS active)
- Time after ROSC confirmed
- Time during ECMO run

**Target CCF**: ≥80% is considered high-quality CPR

**Improving CCF**:
- Minimize pulse check duration
- Use LUCAS device
- Reduce pre-shock pauses
- Limit interruptions

**Adjusting Pulse Check Duration**:
- In End Session form, modify "Pause Duration Per Pulse Check"
- If your team pauses 5 seconds instead of 10, enter "5"
- CCF automatically recalculates
- More accurate CCF helps quality improvement

---

## Settings & Customization

### Metronome Speed
- Access: Hamburger menu → Metronome section
- Options: 100, 110, 120 BPM
- Changes take effect immediately
- Applies to Coach mode only

### Adrenaline Intervals
- Access: Hamburger menu → Adrenaline Interval section
- Options: 3, 4, 5 minutes
- Changes apply to next dose timing
- Does not affect doses already given

### Language Selection
- Access: Hamburger menu → Session Controls → EN/TH toggle
- English: Default voice alerts
- Thai: Thai language voice alerts
- Only affects voice alerts, not interface

### Mode Toggle
- Access: Cycle Tracker panel → Top right switch
- Coach: Green, automatic alerts
- Track: Gray, manual tracking
- Can switch during session (undo available)

---

## Troubleshooting

### Audio Issues

**Metronome Not Playing**:
- Check device is not on silent mode
- Verify volume is turned up
- Check that Coach mode is enabled
- Ensure session is started
- Check that ROSC/ECMO are not active (suppresses audio)

**Metronome Sounds Irregular**:
- This is a known iOS timing limitation
- App uses Web Audio API for best precision
- Minor variations are normal on mobile devices

**Voice Alerts Not Playing**:
- Verify Coach mode is enabled
- Check that alerts are not suppressed (ROSC/ECMO/Session Ended)
- Ensure device volume is up
- Check that soundEnabled is true

### Session Issues

**Cannot Save Session**:
- Must be signed in to save
- Tap "End & Sign In to Save" if you're a guest
- Complete sign-in process
- Try saving again

**Cannot Access Records During Session**:
- This is intentional - records are disabled during active CPR
- End current session first
- Then access Records from menu

**Time Delay Not Showing Correctly**:
- Time delay adds to total CPR time retroactively
- Check that you entered correct minutes
- Time delay total shows in hamburger menu button
- If incorrect, you can add more time (cumulative)

**Duplicate Sessions Saved**:
- Fixed in latest version
- If you see duplicate, it was from double-tapping
- Current version prevents duplicate saves with loading state

### Alert Issues

**Alerts Not Appearing When Expected**:
- Verify you're in Coach mode (not Track mode)
- Check that rhythm is set correctly (shockable vs non-shockable)
- Ensure ROSC/ECMO are not active
- Check adrenaline interval setting

**Cannot Dismiss Medication Alert**:
- Dismiss button only appears in Coach mode
- In Track mode, use "Give" button to log administration
- Ensure session is not ended

### Interface Issues

**Banners Too Small/Text Not Visible**:
- All banners should have same height (110px minimum)
- Font should be bold and size "base"
- If not, try restarting app

**LUCAS Button Not Working**:
- LUCAS toggle is separate from Pulse Check
- Located to the right of Pulse Check banner
- Should be full height (110px minimum)
- Blue when active, gray when inactive

---

## Frequently Asked Questions

### Can I use this app without internet?

Yes. The app works completely offline for tracking CPR. Internet is only required for:
- Signing in
- Saving sessions to cloud
- Syncing records across devices

### How do I switch between Coach and Track mode during a session?

1. Locate the toggle switch in the Cycle Tracker panel (top-right)
2. Tap the switch to toggle
3. Toast notification confirms the mode change
4. "Undo" option available for 4 seconds

### What happens if I accidentally close the app?

**During Active Session**:
- Session state is maintained in browser memory
- Reopen immediately: session continues
- Close for extended time or force quit: session may be lost
- Recommendation: Keep app open during CPR

**Ended Sessions**:
- If saved: safely stored in database
- If not saved: data may be lost
- Always save sessions before closing

### Can I edit session data after saving?

**Editable**:
- Patient demographics (name, HN, hospital, location, sex, age)
- Outcome
- Session notes

**Not Editable**:
- Timeline events (shocks, medications, procedures)
- Timestamps
- Collapse time
- Bystander CPR time
- Total CPR duration
- CCF and statistics

### How is my data stored?

**When Signed In**:
- Sessions saved to Supabase cloud database
- Encrypted in transit and at rest
- Associated with your user account
- Accessible from any device when signed in

**When Not Signed In (Guest)**:
- No session data is saved
- Must sign in to save sessions
- Historical sessions not available

### Can I export my records?

Yes:
1. Open a saved record
2. Tap "Export HTML" button
3. HTML file generated with complete session data
4. Open in any web browser, print, or archive

Export includes:
- Full timeline of events
- All statistics
- Patient demographics
- CCF calculations
- Formatted for professional documentation

### Does the app replace CPR training?

**NO**. This app is a tool to assist trained medical professionals. It is:
- NOT a substitute for proper CPR certification
- NOT intended for use by untrained individuals
- NOT medical advice or diagnostic tool
- NOT a replacement for clinical judgment

Always follow:
- Your institution's protocols
- Current resuscitation guidelines
- Your professional training and judgment

### What if I disagree with the app's medication timing?

The app follows standard protocols, but you should:
- Always follow your institution's specific protocols
- Use clinical judgment
- Override app suggestions when appropriate
- Dismiss alerts that don't apply to your patient
- Configure intervals (adrenaline) to match your protocol

The app is a tool, not a directive.

### Can I use this for pediatric resuscitation?

The app includes pediatric energy selection for defibrillation, but:
- Medication dosing is adult-based
- Timing may differ for pediatrics
- Consult pediatric resuscitation guidelines
- Use clinical judgment for all pediatric cases

### Why is CCF lower than expected?

Common reasons for low CCF:
- Multiple pulse checks (10 seconds each)
- Procedure insertions (ETT = 10 seconds)
- Multiple shocks without LUCAS
- Extended pauses for rhythm checks
- Late ROSC confirmation in app

To improve:
- Minimize pulse check duration (adjust in end form)
- Activate LUCAS toggle when using LUCAS
- Reduce pre-shock pauses
- Confirm ROSC immediately when achieved

---

## Technical Requirements

### Device Requirements
- iOS device (iPhone or iPad)
- iOS version: [Check your current deployment target]
- Web browser with modern JavaScript support
- Recommended: iOS 15.0 or later

### Network Requirements
- **Offline Use**: Fully functional for CPR tracking
- **Online Required**: Sign in and save sessions
- **Bandwidth**: Minimal (text data only)

### Storage
- App size: ~[Check bundle size] MB
- Session data: ~10-50 KB per session
- Records stored in cloud when signed in

### Permissions
- **Notifications**: Optional (for future features)
- **Microphone**: Not required
- **Camera**: Not required
- **Location**: Not required

---

## Data & Privacy

### What Data Is Collected?

**CPR Session Data** (when signed in):
- Event timestamps (shocks, medications, procedures)
- Rhythm selections
- LUCAS usage
- Outcome information
- Patient demographics (if provided by you)
- Session notes (if provided by you)

**User Account Data**:
- Email address
- User ID (generated)
- Session associations

### What Data Is NOT Collected?

- Location data
- Device information
- Usage analytics (no tracking)
- Personal health information beyond what you enter
- Audio recordings
- Photos or videos

### Data Storage

**Cloud Storage** (when signed in):
- Supabase database (PostgreSQL)
- Encrypted in transit (HTTPS)
- Encrypted at rest
- Servers in [Check Supabase region]

**Local Storage**:
- Session state during active CPR (browser memory)
- No persistent local storage for guest users

### Data Sharing

- Data is NOT shared with third parties
- Data is NOT sold
- Data is NOT used for advertising
- Only you can access your session records

### Data Retention

- Session records retained indefinitely while account active
- Delete individual sessions anytime
- Delete account to remove all data

### Your Rights

- Access your data anytime (via Records page)
- Export your data (HTML export per session)
- Delete your data (delete sessions or account)
- Request data portability

For complete privacy details, see our [Privacy Policy](link-to-privacy-policy).

---

## Contact & Support

### Support Email

For assistance, bug reports, or questions:
**Email**: [your-support-email@example.com]

### Bug Reports

When reporting bugs, please include:
- iOS version
- Device model
- App version (see About section)
- Steps to reproduce
- Screenshots if applicable
- What you expected vs. what happened

### Feature Requests

We welcome suggestions for improvements:
- Email us with detailed description
- Explain the use case
- Why it would be valuable

### Response Time

- Support emails: 24-48 hours
- Critical bugs: Priority response
- Feature requests: Acknowledged within 1 week

---

## App Version & Updates

**Current Version**: 1.0.0

### Recent Updates

**Version 1.0.0** (Initial Release):
- Complete CPR tracking with Coach and Track modes
- Medication alerts (Adrenaline, Amiodarone, Lidocaine)
- Configurable metronome (100/110/120 BPM)
- Chest Compression Fraction calculation
- Session saving and records management
- HTML export functionality
- English and Thai voice support
- LUCAS device integration
- ROSC and ECMO support

### Planned Features

- Additional language support
- Custom medication protocols
- Team member tracking
- Enhanced analytics
- Offline-first improvements

---

## Credits

### Development

CPR Timer developed by [Your Name/Organization]

### Medical Consultation

[If you have medical advisors, list them here]

### Open Source

This app uses the following open source libraries:
- React
- Supabase
- Shadcn/ui components
- Lucide icons
- Sonner (toast notifications)

---

## Additional Resources

### Resuscitation Guidelines

Please refer to current guidelines from:
- American Heart Association (AHA)
- European Resuscitation Council (ERC)
- Your local resuscitation council
- Your institution's specific protocols

### Training Resources

For CPR certification and training:
- [Link to AHA courses]
- [Link to local training programs]
- [Your institution's training]

---

## Legal

### Terms of Service

[Link to Terms of Service]

### Privacy Policy

[Link to Privacy Policy]

### Medical Disclaimer

This app is provided "as is" for informational and tracking purposes only. It is not intended to replace professional medical judgment, training, or institutional protocols. The developers make no warranties regarding accuracy, reliability, or fitness for any particular purpose. Use of this app is at your own risk. Always follow current resuscitation guidelines and your institution's protocols.

### Liability

The developers, contributors, and distributors of this app shall not be liable for any clinical decisions made using this tool, or for any outcomes resulting from its use. This app is a supplementary tool for trained medical professionals and does not constitute medical advice.

---

## Updates to This Support Document

This support document may be updated periodically. Check back for:
- New feature documentation
- Updated protocols
- Enhanced troubleshooting guides
- Additional FAQ entries

**Last Updated**: [Date]

---

**Need Help?** Contact us at [your-support-email@example.com]

**Privacy Policy**: [Link]

**Terms of Service**: [Link]
