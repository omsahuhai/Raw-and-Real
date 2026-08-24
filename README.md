# 🍊 RAW & REAL — Fresh Juice, Shake & Salad Bar (Raipur)

> **100% Pure, Fresh & Uncut Goodness in Raipur.**  
> A production-ready, ultra-responsive Single Page Application (SPA) with a thumb-friendly mobile ordering workflow and a direct WhatsApp order engine.

📍 **Location:** Main Food Square, Marine Drive & VIP Road, Raipur, Chhattisgarh — 492001  
🗺️ **Google Maps:** [https://maps.app.goo.gl/So6n6C9E5EzBaEwc7](https://maps.app.goo.gl/So6n6C9E5EzBaEwc7)  
📞 **Order & Support:** [+91 79997 52252](tel:+917999752252)

---

## ✨ Design System & Aesthetic

Inspired by the acclaimed Dribbble concept *"Fresh & Juicy"* by Bac Nguyen:
- **Base Canvas:** Warm ivory and cream mesh gradient (`#FFFDF9` to `#FFF8EE`).
- **5 Category Pastel Colorways:**
  - 🥤 **Shakes:** Soft Strawberry Cream (`#FCE7F3`, text: `#BE185D`, border: `#FBCFE8`)
  - 🍉 **Fruit Salads:** Gentle Peach / Mango (`#FFEDD5`, text: `#C2410C`, border: `#FED7AA`)
  - 🥗 **Veggie & Protein Salads:** Avocado / Mint Green (`#DCFCE7`, text: `#15803D`, border: `#BBF7D0`)
  - 🍊 **Fresh Juices:** Vibrant Tangerine / Citrus (`#FEF3C7`, text: `#B45309`, border: `#FDE68A`)
  - 🧊 **Coolers:** Icy Sky Blue / Mint (`#E0F2FE`, text: `#0369A1`, border: `#BAE6FD`)
- **Brand CTAs:** Energetic Coral (`#EA580C`) and WhatsApp Emerald (`#25D366`).
- **Typography:** Google Fonts `'Plus Jakarta Sans'` (Weights: 400, 500, 600, 700, 800).
- **Cards:** `rounded-3xl` with organic drop shadows (`shadow-organic`) and hover lifts.

---

## 📋 Full Menu Structure (`const MENU_DATA`)

All 40 menu items are managed inside an easily editable JavaScript object array at the top of the `<script>` tag in `index.html`:

| Category | Items Included | Price Range |
| :--- | :--- | :--- |
| **01. Shakes** (12 Items) | Oreo, KitKat, Nutella, Mango, Chocolate, Banana Peanut Butter, Cold Coffee, Brownie, Dry Fruit, Ferrero Rocher, Lotus Biscoff, Badam | ₹110 – ₹180 |
| **02. Fruit Salads** (8 Items) | Classic Mixed Fruit, Dry Fruit & Fresh Fruit, Fruit Chaat, Honey Lime, Yogurt, Exotic Fruit, Tropical Fruit, Sprout Fruit | ₹90 – ₹150 |
| **03. Veggie & Protein Salads** (7 Items) | Sprouts, Protein Veg, Corn & Veg, Garden Fresh, Greek, Coleslaw, Caesar | ₹80 – ₹140 |
| **04. Fresh Juices** (9 Items) | Mosambi, Orange, Watermelon, ABC Juice (Apple, Beetroot, Carrot), Pineapple, Pomegranate, Green Detox, Lemonade, Sugarcane | ₹50 – ₹110 |
| **05. Coolers** (4 Items) | Virgin Mojito, Watermelon Mint, Lemon Mint, Pineapple Mint | ₹80 – ₹90 |

---

## ⚡ Core Features

1. **Sticky Header:**
   - Pulsing live indicator: `🟢 Open Now • Raipur`.
   - Direct phone call shortcut (`tel:+917999752252`).
   - Dynamic Cart trigger button with real-time badge count.

2. **Hero Section & Smart WhatsApp Dialog:**
   - Value propositions: *100% RO Ice*, *Pure Fruits*, *Cold Pressed*, *5-Min Prep*.
   - Clicking **"⚡ Order on WhatsApp"** with an empty cart triggers a theme-matched modal prompt (*"First select any item from the menu"*) with a smooth **"See Menu ↓"** navigation button.
   - If items are already selected, it opens the Order Drawer directly for fast checkout.

3. **Dynamic Filtering & Live Search:**
   - Sticky horizontal category tabs.
   - Real-time search bar that filters across item names, ingredients, and tags.

4. **Interactive Stepper Controls:**
   - `+ Add` button transforms into a `[ - ] [ qty ] [ + ]` stepper with toast notifications on change.

5. **Sticky Floating Cart Bar & WhatsApp Order Drawer:**
   - Displays live item count, subtotal calculation, and `Review Order ➔` button.
   - Order Type selection: **Takeaway**, **Dine-in**, **Stall Pickup**.
   - Custom instructions field (e.g., *"Less ice", "No sugar in juices"*).
   - Generates and encodes structured WhatsApp messages to `+91 79997 52252`:
     ```text
     *NEW ORDER - RAW & REAL RAIPUR* 🍹
     -----------------------------------
     • 2x ABC Juice (₹220)
     • 1x Nutella Shake (₹150)
     -----------------------------------
     *Total Bill:* ₹370
     *Order Type:* Takeaway
     *Special Note:* Less ice in ABC Juice.
     -----------------------------------
     _Sent from Raw & Real Web Menu_
     ```

6. **Location & Google Maps:**
   - Direct button to [Google Maps Location](https://maps.app.goo.gl/So6n6C9E5EzBaEwc7).
   - "Rate Us 5 Stars" review shortcut.

---

## 🚀 Getting Started

### Option 1: Run with Vite (Local Dev Server)
```bash
# Install dependencies (Vite only)
npm install

# Start development server (opens at http://localhost:5173)
npm run dev
```

### Option 2: Standalone Static HTML (Zero Build Step)
Simply open `index.html` in any modern web browser or upload it directly to any static web host (Vercel, Netlify, Cloudflare Pages, GitHub Pages, or Apache/Nginx).

---

## 🛠️ How to Update Menu Items & Prices

Open `index.html` and locate the `const MENU_DATA = [...]` array around line 380:
```javascript
{ 
  id: "fj4", 
  name: "ABC Juice", 
  category: "fresh_juices", 
  price: 110, 
  desc: "Apple, Beetroot, Carrot - Raipur's favorite detox elixir", 
  icon: "🍎", 
  tag: "Skin Glow" 
}
```
Simply edit the `price`, `name`, `desc`, or `tag` to update the website in real-time.

---

## 📄 License
Created for **RAW AND REAL Juice Bar**, Raipur, Chhattisgarh. All rights reserved.
