# Patisserie Nikos Koufos Website 🍰

Ένα premium, σύγχρονο website για το ζαχαροπλαστείο Patisserie Nikos Koufos, εμπνευσμένο από το Choureal.com.

## 🎨 Χαρακτηριστικά

- **Premium Design**: Elegant χρυσό-καφέ χρωματική παλέτα με glassmorphism effects
- **Responsive**: Πλήρως responsive σε όλες τις συσκευές (mobile, tablet, desktop)
- **Smooth Animations**: Fade-in animations, parallax effects, και hover interactions
- **Instagram Integration**: Ενσωματωμένο Instagram feed section
- **Contact Form**: Φόρμα επικοινωνίας με validation
- **SEO Optimized**: Proper meta tags και semantic HTML

## 📁 Δομή Αρχείων

```
nikoskoufos.gr/
├── index.html          # Κύρια σελίδα HTML
├── style.css           # Όλα τα styles και animations
├── script.js           # JavaScript για interactions
├── assets/
│   ├── products/       # Φωτογραφίες προϊόντων (6 εικόνες)
│   └── instagram/      # Instagram feed εικόνες (4 εικόνες)
└── README.md          # Αυτό το αρχείο
```

## 🚀 Πώς να Ανοίξετε το Website

### Μέθοδος 1: Python HTTP Server (Συνιστάται)

```bash
# Ανοίξτε terminal στον φάκελο του project
cd C:\Users\Sgooman\Documents\Projects\nikoskoufos.gr

# Ξεκινήστε τον server
python -m http.server 8000

# Ανοίξτε τον browser στο:
# http://localhost:8000
```

### Μέθοδος 2: Node.js serve

```bash
# Εγκατάσταση (μόνο την πρώτη φορά)
npm install -g serve

# Εκκίνηση server
serve .

# Ανοίξτε τον browser στο URL που εμφανίζεται
```

### Μέθοδος 3: Απλό Άνοιγμα

Απλά κάντε double-click στο `index.html` - αλλά μπορεί να μην λειτουργούν όλα τα features.

## 🎯 Sections του Website

### 1. Hero Section
- Full-screen εισαγωγική σελίδα
- Εντυπωσιακό background με overlay
- Call-to-action buttons
- Animated scroll indicator

### 2. About Section (Η Ιστορία Μας)
- 3 cards με τη φιλοσοφία του ζαχαροπλαστείου
- Fade-in animations on scroll

### 3. Products Section (Οι Δημιουργίες Μας)
- 6 product cards με hover effects
- Κατηγορίες: Τούρτες Γενεθλίων, Γαμήλιες Τούρτες, Μικρά Γλυκά, Σοκολατένιες Δημιουργίες, Παραδοσιακά Γλυκά, Ειδικές Παραγγελίες

### 4. Instagram Section
- 4 Instagram posts με hover overlay
- Link προς το Instagram profile
- Dark background για contrast

### 5. Contact Section (Επικοινωνήστε Μαζί Μας)
- Πληροφορίες επικοινωνίας (διεύθυνση, τηλέφωνο, email, ωράριο)
- Contact form με validation

### 6. Footer
- Social media links (Instagram, Facebook)
- Quick links navigation
- Copyright information

## 🎨 Χρωματική Παλέτα

- **Primary Gold**: #D4AF37 (Κύριο χρυσό)
- **Gold Light**: #F4E4C1 (Ανοιχτό χρυσό)
- **Brown Dark**: #3E2723 (Σκούρο καφέ)
- **Brown Medium**: #5D4037 (Μεσαίο καφέ)
- **Cream**: #FFF8E7 (Κρεμ)
- **Accent**: #C2185B (Έμφαση)

## 📱 Responsive Breakpoints

- **Desktop**: > 768px
- **Tablet**: 768px
- **Mobile**: < 480px

## ✨ Features & Interactions

### Navigation
- Fixed navbar που γίνεται transparent στο top
- Smooth scroll σε όλα τα sections
- Mobile hamburger menu
- Active link highlighting

### Animations
- Fade-in on scroll για όλα τα sections
- Parallax effect στο hero
- Hover effects στα product cards
- Smooth transitions παντού

### Form
- Real-time validation
- Custom notification system
- Email format checking

## 🔧 Προσαρμογές που Μπορείτε να Κάνετε

### Αλλαγή Φωτογραφιών
Αντικαταστήστε τις εικόνες στους φακέλους:
- `assets/products/product1.jpg` έως `product6.jpg`
- `assets/instagram/ig1.jpg` έως `ig4.jpg`

### Αλλαγή Χρωμάτων
Επεξεργαστείτε τις CSS variables στο `style.css` (γραμμές 10-30):
```css
:root {
  --color-primary-gold: #D4AF37;
  --color-brown-dark: #3E2723;
  /* κλπ */
}
```

### Αλλαγή Κειμένων
Επεξεργαστείτε το `index.html` και αλλάξτε τα κείμενα στα sections.

### Προσθήκη Google Maps
Στο Contact section, μπορείτε να προσθέσετε embedded Google Map:
```html
<iframe src="YOUR_GOOGLE_MAPS_EMBED_URL" width="100%" height="400"></iframe>
```

## 📧 Contact Form Backend

Το contact form προς το παρόν δεν στέλνει emails. Για να το ενεργοποιήσετε:

### Επιλογή 1: Formspree (Εύκολο)
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Επιλογή 2: EmailJS (JavaScript)
Προσθέστε το EmailJS library και configure στο `script.js`

### Επιλογή 3: Backend Server
Δημιουργήστε ένα backend endpoint (Node.js, PHP, κλπ)

## 🌐 Deployment

### GitHub Pages
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin YOUR_REPO_URL
git push -u origin main
```
Ενεργοποιήστε GitHub Pages στα settings.

### Netlify
1. Drag & drop τον φάκελο στο netlify.com
2. Ή συνδέστε το GitHub repo

### Vercel
```bash
npm install -g vercel
vercel
```

## 📝 To-Do List (Προαιρετικά)

- [ ] Προσθήκη Google Analytics
- [ ] Προσθήκη Google Maps στο Contact
- [ ] Live Instagram feed integration (API)
- [ ] Multilingual support (EN/GR)
- [ ] Blog section για νέα προϊόντα
- [ ] Online ordering system
- [ ] Cookie consent banner
- [ ] Performance optimization (image compression)

## 🐛 Troubleshooting

### Οι εικόνες δεν φορτώνουν
- Ελέγξτε ότι τα paths είναι σωστά
- Βεβαιωθείτε ότι τρέχετε local server (όχι απλό file://)

### Το mobile menu δεν λειτουργεί
- Ελέγξτε το browser console για errors
- Βεβαιωθείτε ότι το `script.js` φορτώνει σωστά

### Animations δεν παίζουν
- Κάντε hard refresh (Ctrl+F5)
- Ελέγξτε αν το CSS φορτώνει

## 📞 Support

Για οποιαδήποτε ερώτηση ή πρόβλημα, ανατρέξτε στα αρχεία:
- `style.css` - Όλα τα styles
- `script.js` - Όλη η λειτουργικότητα
- `index.html` - Δομή σελίδας

## 🎉 Enjoy!

Το website σας είναι έτοιμο! Απλά προσθέστε τις δικές σας φωτογραφίες και κείμενα και είστε έτοιμοι για launch! 🚀🍰
