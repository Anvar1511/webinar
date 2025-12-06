# 🎯 WEBINAR LANDING PAGE - UNIVERSAL SHABLON

Professional, conversion-optimized webinar landing page shabloni. Tez va oson sozlash imkoniyati bilan.

---

## 📁 Fayl strukturasi

```
webinar-template/
├── index.html          # Asosiy HTML fayl
├── css/
│   └── styles.css      # Barcha stillar
├── js/
│   ├── config.js       # ⭐ ASOSIY - Barcha sozlamalar
│   └── script.js       # Funksionallik
├── img/
│   ├── mentor.svg      # Mentor rasmi (placeholder)
│   ├── favicon.svg     # Favicon
│   ├── flag-uz.svg     # O'zbekiston bayrog'i
│   ├── flag-ru.svg     # Rossiya bayrog'i
│   ├── flag-kz.svg     # Qozog'iston bayrog'i
│   ├── flag-tj.svg     # Tojikiston bayrog'i
│   └── flag-kg.svg     # Qirg'iziston bayrog'i
└── README.md           # Qo'llanma (shu fayl)
```

---

## 🚀 TEZKOR BOSHLASH

### 1-qadam: config.js ni oching

`js/config.js` faylini istalgan matn muharririda oching (VS Code, Notepad++, yoki boshqa).

### 2-qadam: Asosiy ma'lumotlarni o'zgartiring

```javascript
const CONFIG = {
    webinar: {
        pageTitle: "Sizning webinar sarlavhangiz",
        headline: "Asosiy sarlavha",
        subheadline: "Qisqacha tavsif",
        category: "Kategoriya",
        date: "15-16 dekabr",
        time: "20:30",
    },
    
    mentor: {
        name: "Mentor ismi",
        title: "Mutaxassislik",
        photo: "img/mentor.webp", // O'z rasmingizni qo'ying
        bio: "Qisqacha bio"
    },
    
    // ... boshqa sozlamalar
};
```

### 3-qadam: Rasmlarni almashtiring

`img/` papkasiga quyidagilarni joylashtiring:
- `mentor.webp` - Mentor rasmi (tavsiya: 400x400px)
- `og-image.jpg` - Ijtimoiy tarmoqlar uchun rasm (1200x630px)

### 4-qadam: Saytni tekshiring

`index.html` ni brauzerda oching va tekshiring.

---

## ⚙️ BATAFSIL SOZLAMALAR

### 💰 Narx va chegirma

```javascript
pricing: {
    originalPrice: "299 000",    // Eski narx (chiziladi)
    currentPrice: "BEPUL",       // Hozirgi narx
    currency: "so'm",
    discount: "100%"             // Chegirma foizi
}
```

### ⏰ Timer va urgency

```javascript
urgency: {
    spotsLeft: 47,               // Qolgan joylar
    totalSpots: 100,             // Jami joylar
    timerHours: 23,              // Timer soatlar
    timerMinutes: 59,
    timerSeconds: 59,
    urgencyText: "Shoshiling! Joylar soni oz qoldi"
}
```

**Yoki aniq sana bo'yicha:**
```javascript
urgency: {
    timerEndDate: "2024-12-15T20:30:00",  // ISO format
    // ...
}
```

### 📚 Webinarda nima o'rganiladi

```javascript
benefits: [
    {
        icon: "🎯",
        title: "Sarlavha",
        description: "Tavsif"
    },
    // Ko'proq qo'shing...
]
```

**Mavjud emoji ikonkalar:**
🎯 📝 🧠 ⏰ 💡 🔥 ✅ 📊 💰 🚀 📱 🎓 💬 ❓ 🎁 👥 📈 🔑

### 🎁 Sovg'alar

```javascript
gifts: {
    enabled: true,  // false = o'chirish
    title: "Qatnashuvchilar uchun sovg'alar:",
    items: [
        "📘 PDF qo'llanma",
        "🎥 Video dars",
        "📋 Shablon",
        "✅ Bonus"
    ]
}
```

### 💬 Testimoniallar

```javascript
testimonials: {
    enabled: true,
    title: "Qatnashuvchilar fikrlari:",
    items: [
        {
            name: "Ism F.",
            role: "Lavozim/status",
            photo: "img/testimonial-1.webp", // yoki null
            text: "Sharh matni...",
            rating: 5  // 1-5
        }
    ]
}
```

### ❓ Ko'p so'raladigan savollar (FAQ)

```javascript
faq: {
    enabled: true,
    title: "Ko'p so'raladigan savollar",
    items: [
        {
            question: "Savol?",
            answer: "Javob."
        }
    ]
}
```

### 📊 Statistika (Social Proof)

```javascript
stats: {
    enabled: true,
    items: [
        { number: "500+", label: "O'quvchi" },
        { number: "95%", label: "Qoniqish" },
        { number: "10+", label: "Yil tajriba" },
        { number: "50+", label: "Bugun ro'yxatdan" }
    ]
}
```

### 🎨 Dizayn sozlamalari

```javascript
design: {
    // Ranglar
    primaryColor: "#E63946",      // CTA tugmalar (qizil)
    secondaryColor: "#1D3557",    // Sarlavhalar (ko'k)
    accentColor: "#F4A261",       // Accent (sariq)
    backgroundColor: "#F8F9FA",   // Fon
    
    // Gradient (hero section)
    gradientStart: "#1D3557",
    gradientEnd: "#457B9D",
    
    // Shriftlar (Google Fonts)
    headingFont: "'Montserrat', sans-serif",
    bodyFont: "'Open Sans', sans-serif",
    
    // Animatsiyalar
    animationsEnabled: true
}
```

**Tavsiya etiladigan rang kombinatsiyalari:**

| Nom | Primary | Secondary | Accent |
|-----|---------|-----------|--------|
| Klassik | #E63946 | #1D3557 | #F4A261 |
| Yashil | #10B981 | #064E3B | #FCD34D |
| Binafsha | #7C3AED | #1F2937 | #F59E0B |
| Ko'k | #2563EB | #1E3A5F | #F97316 |

### 📊 Analytics

```javascript
analytics: {
    facebookPixelId: "YOUR_PIXEL_ID",
    googleAnalyticsId: "G-XXXXXXXXXX",
    yandexMetrikaId: "",
    tiktokPixelId: ""
}
```

### 📝 Forma sozlamalari

```javascript
form: {
    nameEnabled: false,        // Ism maydoni
    emailEnabled: false,       // Email maydoni
    submitButton: "BEPUL QATNASHISH",
    
    // Webhook URL (Google Sheets, Zapier, etc.)
    actionUrl: "https://your-webhook-url.com/submit",
    
    // Yoki Telegram bot
    telegramBotToken: "BOT_TOKEN",
    telegramChatId: "CHAT_ID"
}
```

---

## 🔗 FORMA MA'LUMOTLARINI QABUL QILISH

### Variant 1: Telegram bot orqali

1. @BotFather dan bot yarating
2. Bot tokenini oling
3. Chat ID ni aniqlang
4. config.js ga qo'ying:

```javascript
form: {
    telegramBotToken: "123456789:ABCdefGHIjklMNOpqrsTUVwxyz",
    telegramChatId: "-1001234567890"
}
```

### Variant 2: Google Sheets + Google Apps Script

1. Google Sheets yarating
2. Extensions → Apps Script
3. Quyidagi kodni joylashtiring:

```javascript
function doPost(e) {
  var sheet = SpreadsheetApp.getActiveSheet();
  var data = JSON.parse(e.postData.contents);
  
  sheet.appendRow([
    new Date(),
    data.phone,
    data.name,
    data.email,
    data.source
  ]);
  
  return ContentService.createTextOutput('OK');
}
```

4. Deploy → Web app
5. URL ni config.js ga qo'ying

### Variant 3: Zapier/Make webhook

1. Zapier yoki Make da webhook trigger yarating
2. URL ni config.js ga qo'ying

---

## 📱 HOSTING

### Variant 1: Vercel (Tavsiya etiladi - BEPUL)

1. [vercel.com](https://vercel.com) ga ro'yxatdan o'ting
2. GitHub repositoriyangizni ulang yoki fayllarni yuklang
3. Deploy tugmasini bosing
4. Tayyor! URL: `your-project.vercel.app`

### Variant 2: Netlify (BEPUL)

1. [netlify.com](https://netlify.com) ga ro'yxatdan o'ting
2. "Sites" → "Drag and drop" ga papkani tashlang
3. Tayyor!

### Variant 3: GitHub Pages (BEPUL)

1. GitHub da repository yarating
2. Settings → Pages → Source: main branch
3. Tayyor! URL: `username.github.io/repo-name`

### Variant 4: Oddiy hosting

Fayllarni FTP orqali hostingga yuklang.

---

## ✅ CHECKLIST - LAUNCH OLDIDAN

- [ ] config.js dagi barcha ma'lumotlar to'g'ri
- [ ] Mentor rasmi yuklangan (img/mentor.webp)
- [ ] OG image yuklangan (img/og-image.jpg)
- [ ] Facebook Pixel ID qo'yilgan
- [ ] Forma webhook/Telegram sozlangan
- [ ] Barcha havolalar ishlayapti
- [ ] Mobile versiya tekshirilgan
- [ ] Timer to'g'ri ishlayapti
- [ ] Forma yuborish ishlayapti

---

## 🆘 MUAMMOLAR VA YECHIMLAR

### Timer ishlamayapti
- Browser console da xatolik bor-yo'qligini tekshiring (F12)
- config.js dagi timer sozlamalarini tekshiring

### Rasmlar ko'rinmayapti
- Fayl nomlari to'g'ri yozilganini tekshiring
- Fayl kengaytmasi to'g'ri bo'lishi kerak (.webp, .jpg, .png)

### Forma ishlamayapti
- actionUrl yoki Telegram sozlamalarini tekshiring
- Browser console da xatolikni ko'ring

### Stillar noto'g'ri ko'rinadi
- CSS fayli to'g'ri ulanganni tekshiring
- Browser keshini tozalang (Ctrl+Shift+R)

---

## 📞 QISQA LOYIHA NOMI NAMUNALARI

Har xil webinarlar uchun config.js dan tez o'zgartirish:

### Ta'lim webinari
```javascript
webinar: {
    headline: "IELTS 7.0+ ga 3 oyda chiqish sirlari",
    category: "IELTS tayyorgarlik",
    date: "20-21 dekabr"
}
```

### Marketing webinari
```javascript
webinar: {
    headline: "Instagram orqali oyiga $3000+ topish",
    category: "SMM Marketing",
    date: "15 dekabr"
}
```

### Biznes webinari
```javascript
webinar: {
    headline: "0 dan online biznes ochish yo'l xaritasi",
    category: "Biznes",
    date: "10-11 yanvar"
}
```

---

## 📝 VERSIYA TARIXI

- **v1.0.0** (Dekabr 2024) - Birinchi reliz
  - Professional dizayn
  - Timer va urgency elementlar
  - Testimoniallar slider
  - FAQ accordion
  - Mobile-optimized
  - Facebook Pixel ready
  - Telegram bot integratsiya

---

## 🤝 YORDAM

Savollar yoki takliflar bo'lsa, bog'laning.

---

**Muvaffaqiyatli webinarlar tilaymiz! 🚀**
