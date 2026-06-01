# 🕐 Digital Clock - Multi Timezone Display

A beautiful, responsive digital clock application that displays the current time in multiple time zones around the world with real-time updates.

## ✨ Features

- ✅ **Real-time Updates** - Clock updates every second
- ✅ **Multi Timezone Support** - Display clocks for different time zones
- ✅ **Add/Remove Timezones** - Customize which timezones to display
- ✅ **UTC Offset Display** - See the UTC offset for each timezone
- ✅ **AM/PM Indicator** - Period information for 12-hour format
- ✅ **Date Display** - Full date for each timezone
- ✅ **Persistent Storage** - Your timezone preferences are saved locally
- ✅ **Responsive Design** - Works on desktop, tablet, and mobile
- ✅ **Smooth Animations** - Beautiful transitions and effects
- ✅ **Quick Add Buttons** - Pre-configured popular timezones

## 🚀 Quick Start

### Option 1: Open in Browser (Easiest)
Simply open `index.html` in your web browser:
```bash
# Double-click index.html or
open index.html
```

### Option 2: Use Live Server (Recommended)
```bash
# If you have Python 3 installed
python -m http.server 8000

# Then visit http://localhost:8000
```

### Option 3: Use Node.js http-server
```bash
npm install -g http-server
http-server
# Visit http://localhost:8080
```

## 📁 Project Structure

```
digital-clock/
├── index.html          # HTML structure
├── styles.css          # CSS styling and animations
├── script.js           # JavaScript logic
└── README.md          # This file
```

## 🎯 How to Use

### Adding a Timezone

1. **Using the Input Field:**
   - Type a timezone name (e.g., `America/New_York`)
   - Click "Add Timezone" or press Enter
   - The clock will appear immediately

2. **Using Quick Add Buttons:**
   - Scroll down to "Suggested Timezones"
   - Click on any city to add it instantly

### Removing a Timezone

1. Hover over any clock card
2. Click the "✕" button in the top-right corner
3. The timezone will be removed

### Resetting to Default

- Click "Reset to Default" button
- Restores the default timezones: Bangkok, New York, London, Tokyo

## 🌍 Supported Timezones

Common timezone formats:
- **Americas:** `America/New_York`, `America/Los_Angeles`, `America/Mexico_City`
- **Europe:** `Europe/London`, `Europe/Paris`, `Europe/Berlin`, `Europe/Moscow`
- **Asia:** `Asia/Bangkok`, `Asia/Tokyo`, `Asia/Hong_Kong`, `Asia/Dubai`, `Asia/Singapore`
- **Australia:** `Australia/Sydney`, `Australia/Melbourne`, `Australia/Brisbane`
- **Africa:** `Africa/Cairo`, `Africa/Lagos`, `Africa/Johannesburg`

**Tip:** Most timezone names follow the format `Continent/City`

## 💾 Local Storage

Your preferred timezones are automatically saved to your browser's local storage. When you return to the site, your selected timezones will be remembered!

## 🎨 Design Features

- **Gradient Background:** Beautiful purple gradient background
- **Card-based Layout:** Each timezone displayed in its own card
- **Hover Effects:** Cards lift up when you hover over them
- **Smooth Animations:** Fade-in animations on page load
- **Responsive Grid:** Automatically adjusts for different screen sizes
- **Dark Mode Friendly:** Readable on all backgrounds

## 📱 Responsive Breakpoints

- **Desktop (1200px+):** Multi-column grid layout
- **Tablet (768px+):** 2-column layout
- **Mobile (<768px):** Single column layout

## 🔧 Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Flexbox, Grid, Animations
- **JavaScript ES6+** - Intl API for timezone handling
- **LocalStorage API** - Data persistence

## 📊 Information Displayed

Each clock card shows:
- **Timezone Name** - City/region name
- **Region** - Continent/area
- **Time** - Current time in HH:MM:SS format (24-hour)
- **Date** - Full date with weekday
- **Period** - AM or PM
- **UTC Offset** - Time difference from UTC

## 🛠 Browser Compatibility

- ✅ Chrome/Chromium (90+)
- ✅ Firefox (88+)
- ✅ Safari (14+)
- ✅ Edge (90+)
- ✅ Mobile browsers

## 💡 Tips & Tricks

1. **Add Multiple Timezones:** Create a custom dashboard for teams across different regions
2. **Use for Scheduling:** Quickly find available meeting times
3. **Travel Planning:** Add timezones before your trip
4. **International Business:** Monitor business hours across regions

## 🎓 Learning Points

This project demonstrates:
- JavaScript's Intl API for timezone handling
- CSS Grid and Flexbox layouts
- LocalStorage for data persistence
- DOM manipulation and event handling
- Responsive design principles
- CSS animations and transitions

## 📝 Example Timezones

| City | Timezone | Offset |
|------|----------|--------|
| Bangkok | Asia/Bangkok | +7:00 |
| New York | America/New_York | -5:00 or -4:00 |
| London | Europe/London | +0:00 or +1:00 |
| Tokyo | Asia/Tokyo | +9:00 |
| Sydney | Australia/Sydney | +10:00 |
| Dubai | Asia/Dubai | +4:00 |
| Singapore | Asia/Singapore | +8:00 |
| Los Angeles | America/Los_Angeles | -8:00 or -7:00 |

*Note: Offsets vary based on daylight saving time*

## 🐛 Troubleshooting

**Q: The clock isn't updating**
- A: Refresh the page or check browser console for errors

**Q: "Invalid timezone" error**
- A: Check the timezone name - use format like `Continent/City`

**Q: Changes aren't saved**
- A: Make sure browser allows LocalStorage. Try clearing cache if it persists.

**Q: Clock shows wrong time**
- A: Check your computer's system time is correct

## 🚀 Future Enhancements

Possible improvements:
- [ ] Dark mode toggle
- [ ] Analog clock display option
- [ ] Alarm functionality
- [ ] World map with timezones
- [ ] Export/import timezone preferences
- [ ] Timezone search/autocomplete
- [ ] Multiple clock formats
- [ ] Sound effects

## 📄 License

MIT License - Feel free to use and modify!

## 👤 Author

Created for Honda Thailand Digital Project

## 🤝 Contributing

Feel free to fork, modify, and improve this project!

---

**Live Demo:** Open `index.html` in your browser right now! 🎉
