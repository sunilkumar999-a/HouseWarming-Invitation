# Abburi's Housewarming Invitation

A beautiful, professional housewarming invitation system with personalized guest experience.

## Files

- `index.html` - Main invitation page with envelope cover and wax seal
- `invite-generator.html` - Guest management and personalized link generator
- `send_invites.py` - WhatsApp invitation sender script
- `sw.js` - Service worker for PWA functionality

## Features

- **Beautiful Design** - Wedding-invite-source quality styling
- **Personalized Invitations** - Guest names appear on envelope
- **Wax Seal** - Custom "Abburi's" wax seal with gold design
- **Guest Management** - Add guests and generate personalized links
- **WhatsApp Integration** - Send invitations via WhatsApp
- **Responsive Design** - Works on all devices

## Usage

### Local Testing
```bash
# Start local server
python -m http.server 8000

# Open in browser
http://localhost:8000/index.html
http://localhost:8000/invite-generator.html
```

### Personalized URLs
```
# Main invitation
http://localhost:8000/index.html

# Personalized (example with guest "sunil")
http://localhost:8000/index.html?guest=c3VuaWw=&lang=en
```

### WhatsApp Invitations
```bash
# Generate CSV from invite-generator.html
# Then run:
python send_invites.py
```

## Deployment

Deploy to GitHub Pages or any static hosting service.

## Design

- **Colors** - Gold, navy blue, and cream theme
- **Fonts** - Cinzel, Cormorant Garamond, Great Vibes
- **Layout** - Envelope cover with wax seal reveal
- **Animations** - Smooth transitions and effects

## Guest Personalization

Guest names are Base64 encoded in URLs:
- `guest=c3VuaWw=` = "sunil"
- `guest=c3VuaWwgY2hvd2Rhcnk=` = "sunil chowdary"

Use the invite-generator.html to create personalized links for all guests.
