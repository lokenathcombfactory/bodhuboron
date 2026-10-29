# শুভ বধূবরণ ও বউভাত — ডিজিটাল নিমন্ত্রণপত্র

অভিরাম নাথ ও মোনালিসা দেবনাথের শুভ বধূবরণ ও বউভাত অনুষ্ঠানের জন্য তৈরি ডিজিটাল নিমন্ত্রণপত্র (Digital Bengali Wedding Invitation Card)।

## 🚀 Vercel-এ ডিপ্লয় করার উপায় (How to Deploy to Vercel)

প্রজেক্টটিতে ইতিমধ্যেই `vercel.json`, `package.json`, এবং `.gitignore` কনফিগার করা রয়েছে। আপনি নিচের যেকোনো একটি উপায়ে ডিপ্লয় করতে পারেন:

---

### উপায় ১: Vercel CLI দিয়ে (সবচেয়ে সহজ ও দ্রুত)

টার্মিনাল বা PowerShell খুলে এই ফোল্ডারে রান করুন:

```bash
npx vercel
```

- প্রথমবার রান করলে Vercel লগইন করতে বলবে (Email/GitHub দিয়ে কনফার্ম করুন)।
- প্রশ্নগুলোর উত্তর দিতে Enter চাপুন:
  - `Set up and deploy?` -> **Y**
  - `Which scope?` -> (আপনার অ্যাকাউন্ট সিলেক্ট করুন)
  - `Link to existing project?` -> **N**
  - `Project name?` -> **boubhat-invitation** (বা যেকোনো নাম)
  - `In which directory is your code located?` -> **./** (Enter চাপুন)
- মাত্র কয়েক সেকেন্ডেই আপনার লাইভ লিংক (`https://boubhat-invitation.vercel.app`) তৈরি হয়ে যাবে!

Production-এ লাইভ করার জন্য:
```bash
npx vercel --prod
```

---

### উপায় ২: GitHub-এর মাধ্যমে

1. GitHub-এ একটি নতুন Repository তৈরি করুন।
2. কোড পুশ করুন:
   ```bash
   git add .
   git commit -m "Boubhat digital invitation card ready for Vercel"
   git branch -M main
   git remote add origin https://github.com/<আপনার-ইউজারনেম>/<রেপো-নাম>.git
   git push -u origin main
   ```
3. [vercel.com](https://vercel.com)-এ যান।
4. **Add New...** -> **Project** -> GitHub রিপোজিটরিটি সিলেক্ট করে **Deploy** বাটনে ক্লিক করুন।

---

### উপায় ৩: Vercel Dashboard Drag & Drop

1. [vercel.com/new](https://vercel.com/new)-এ যান।
2. এই সম্পূর্ণ ফোল্ডারটি ড্র্যাগ করে আপলোড বক্সে ছেড়ে দিন।
3. **Deploy** বাটনে ক্লিক করুন।

---

## 📁 ফাইল পরিচিতি
- `index.html`: মূল নিমন্ত্রণপত্র (HTML, CSS, JS ও SVG)
- `boy.webp`: বরের ছবি (অভিরাম নাথ)
- `girl.webp`: কনের ছবি (মোনালিসা দেবনাথ)
- `food.webp`: বউভাত প্রীতিভোজের ছবি
- `music.mp3`: মাঙ্গলিক সানাই/সান্ধ্য সুর
- `curtain-header.jpg`: উপরের উৎসবমুখর লাল রেশমি ঝালর
- `vercel.json`: Vercel ক্যাশিং ও সিকিউরিটি কনফিগারেশন
