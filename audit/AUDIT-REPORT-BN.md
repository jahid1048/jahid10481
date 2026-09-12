# Vital Tips Daily — সম্পূর্ণ SEO ও টেকনিক্যাল অডিট রিপোর্ট (৩৪টি আর্টিকেল)
**সাইট:** https://vitaltipsdaily.blogspot.com
**অডিট তারিখ:** ২০২৬-০৯-১২
**থিম:** vitaltipsdaily-theme-seo-fixed-v19 (থিম XML ফাইলটি আমার কাছে পৌঁছায়নি — শুধু লাইভ রেন্ডার দেখে যাচাই করা হয়েছে)

---

## সারসংক্ষেপ

| অবস্থা | সংখ্যা |
|--------|--------|
| ✅ সম্পূর্ণ ঠিক আছে | ১টি (Circadian Rhythm Reset) |
| 🛠️ সম্পূর্ণ ফিক্স করা হয়েছে | ৩টি (Berberine, Healthy Plate, Cortisol Belly) |
| 🔴 ক্রিটিক্যাল (ইনলাইন CSS / ভাঙা রেন্ডারিং / ইনজেক্টেড স্ক্রিপ্ট) | ১৩টি |
| 🟠 স্ট্রাকচার/SEO সমস্যা (ছবি-প্যারাগ্রাফ-TOC ক্রম ভুল, কমেন্ট ব্লক, সোর্স নেই) | ২০টি |
| 🔁 ডুপ্লিকেট কন্টেন্ট | ২টি (High Fiber জোড়া) |

**এই টার্নে সম্পূর্ণ ফিক্স করা হয়েছে:** ২টি (নিচে ফাইল দেওয়া আছে)
**বাকি:** ব্যাচে ব্যাচে ফিক্স করা হবে (প্রায়োরিটি লিস্ট নিচে)

---

## সবচেয়ে বড় সমস্যাগুলো (সিস্টেমেটিক)

### ১. ১৩টি আর্টিকেলে `<style>` ব্লক ঢুকিয়ে দেওয়া হয়েছে 🔴
পোস্টের ভেতরে ইনলাইন থিম-সিএসএস থাকার কারণে:
- পেজ সাইজ ৪–৮ কেবি করে বাড়ছে (স্পিড/SEO ক্ষতি)
- ২টি পোস্টে `body {}` ও `html, body {}` গ্লোবাল সিলেক্টর আছে — পুরো পেজের লেআউট ভাঙছে:
  - **10 Evidence-Based Health Tips** (body সিলেক্টর)
  - **Post-Meal Walking / Strength Training** (body সিলেক্টর)
  - **Candida auris** (`html, body` + `!important` ওভাররাইড)
- থিম v19 ইতিমধ্যে এসব ক্লাস স্টাইল করে — পোস্টের ভেতরের সিএসএস অপ্রয়োজনীয় ও দ্বন্দ্ব তৈরি করে

### ২. ভুল ক্রম: ফিচার্ড ইমেজ → প্যারাগ্রাফ → টেবিল অফ কন্টেন্ট
আপনার চাওয়া ক্রম অনুযায়ী মাত্র ১টি আর্টিকেল (Circadian) সঠিক। বাকিগুলোর সমস্যা:
- **Natural GLP-1 Foods:** ছবি আছে কিন্তু ইন্ট্রো প্যারাগ্রাফের আগেই TOC; ডিসক্লেইমার উপরে চলে এসেছে
- **Cortisol Belly:** ছবির পর ইন্ট্রো প্যারাগ্রাফ নেই, সরাসরি TOC
- **Creatine/Magnesium/Mobility/Protein/Grip/Anti-inflammatory/Evening Routine:** ছবির পর ইন্ট্রো প্যারাগ্রাফ ও টিওসি নেই — সরাসরি Key Takeaways
- **Fibermaxxing / Sleep Hygiene / Fix Sleep Schedule / Heart-Healthy / 7-Day Meal Plan:** প্যারাগ্রাফ দিয়ে শুরু — ফিচার্ড ইমেজ প্রথমে নেই

### ৩. ৯টি আর্টিকেলে `<!-- Primary Keyword... -->` SEO ব্রিফ কমেন্ট 🔴
গুট-হেলথ, হাই-ফাইবার (২টি), লুজ-ওয়েট, ৯-ফুডস-বিপি — এদের সোর্স কোডে কিওয়ার্ড প্ল্যান ভেসিবেল। গুগল কমেন্ট ইগনোর করলেও এটা প্রফেশনাল নয় ও কখনো কখনো কিওয়ার্ড স্টাফিং সিগন্যাল দেয়। সব মুছতে হবে।

### ৪. ডুপ্লিকেট কন্টেন্ট 🔁
**দুইটি আর্টিকেল একই প্রাইমারি কিওয়ার্ড টার্গেট করছে:**
- #16 "High Fiber Foods for Digestion **and Gut Health**" (আপডেট ০৫ সেপ্ট)
- #17 "High Fiber Foods for Digestion **That Actually Work**" (২৭ আগস্ট, পুরনো)

**সুপারিশ:** #16 রেখে দিন (নতুন, আপডেটেড)। #17-কে হয়:
- (ক) সম্পূর্ণ ভিন্ন অ্যাঙ্গেলে রিরাইট করুন (যেমন: "Fiber Foods vs Supplements: Which Works Better") অথবা
- (খ) ডিলিট করে Blogger সেটিংসে #16-তে 301 রিডাইরেক্ট দিন (সবচেয়ে নিরাপদ SEO সমাধান)

### ৫. স্লাগ (URL) সমস্যা
- `how-to-lose-weight-fast-naturally_0802718094.html` — স্লাগ কলিশন স্যাফিক্স (ডুপ্লিকেট স্লাগের প্রমাণ)
- `a-person-sitting-calmly-outdoors-in.html` ও `wooden-gavel-beside-prescription.html` — ছবির বর্ণনা স্লাগ হয়ে গেছে (Mental Health ও Retatrutide পোস্ট)। **সতর্কতা:** পোস্ট পারমালিংক পরিবর্তনে পুরনো লিংক ভাঙতে পারে; পরিবর্তন করলে অবশ্যই রিডাইরেক্ট ম্যাপ করতে হবে। অন্য পোস্ট থেকে এদের দিকে ইন্টারনাল লিংক আছে (যেমন Berberine থেকে Retatrutide-এর দিকে)।

### ৬. সোর্স লিংক দুর্বল / অনুপস্থিত
- **Berberine:** PubMed/Nature-এর শুধু হোমপেজ লিংক ছিল — নির্দিষ্ট স্টাডির নয় (ফিক্স করা হয়েছে: আসল DOI লিংক বসানো হয়েছে)
- **Healthy Plate:** কোনো সোর্স বক্সই ছিল না (ফিক্স করা হয়েছে: Harvard Nutrition Source, NIH NIDDK, CDC, ADA লিংক যোগ)
- **Alcohol Cancer:** `[38][50]` জাতীয় ব্র্যাকেট সাইটেশন মার্কার রয়ে গেছে কিন্তু লিংক নেই — এগুলো হয় আসল লিংকে বদলাতে হবে নয়তো মুছতে হবে

### ৭. ইনজেক্টেড ম্যালিশাস/জাঙ্ক স্ক্রিপ্ট 🔴
- **Berberine** পোস্টের শেষে Cloudflare challenge-platform `<script>` ঢুকে গিয়েছিল (কপি-পেস্টের সময়)। ফিক্সড ফাইলে মুছে দেওয়া হয়েছে। বাকি পোস্টেও এমন আছে কিনা প্রতিটি ফিক্সের সময় চেক করা হচ্ছে।

### ৮. হটলিংকড ইমেজ
- **Healthy Plate**-এর ফিচার্ড ইমেজ সরাসরি Unsplash থেকে লোড হচ্ছে (`images.unsplash.com`)। কাজ করে, কিন্তু ঝুঁকিপূর্ণ (হটলিংক ভেঙে যেতে পারে, থাম্বনেইল/ওপেন গ্রাফে ধরা পড়ে না)। সার্চ কনসোলে ইমেজ ইনডেক্সিংয়ের জন্য ছবিটি Blogger-এ আপলোড করে সেই URL বসানো ভালো।

---

## পোস্ট-বাই-পোস্ট স্ট্যাটাস টেবিল

| # | আর্টিকেল | সমস্যা | ফিক্স স্ট্যাটাস |
|---|----------|--------|----------------|
| 1 | Circadian Rhythm Reset | কিছু নেই — গোল্ড স্ট্যান্ডার্ড | ✅ লাগবে না |
| 2 | Berberine | `<style>` ব্লক, ছবি নিচে, জাঙ্ক স্ক্রিপ্ট, দুর্বল সোর্স লিংক | ✅ **ফিক্সড: `fixed-posts/02-berberine-FIXED.html`** |
| 3 | Healthy Plate | `<style>` ব্লক, float লেআউট, সোর্স বক্স নেই, Unsplash হটলিংক | ✅ **ফিক্সড: `fixed-posts/03-healthy-plate-FIXED.html`** |
| 4 | Natural GLP-1 Foods | ইন্ট্রোর আগে TOC, ডিসক্লেইমার উপরে, প্রচুর ইনলাইন স্টাইল, র‍্যাপার ডিভ | ⏳ ব্যাচ-২ (টপ প্রায়োরিটি) |
| 5 | Cortisol Belly | ইন্ট্রো প্যারাগ্রাফ নেই, ডিসক্লেইমার উপরে, ইনলাইন স্টাইল | ✅ **ফিক্সড: `fixed-posts/05-cortisol-belly-FIXED.html`** |
| 6 | Alcohol Cancer | `[38][50]` সাইটেশন মার্কার ঝুলে আছে, TOC নেই | ⏳ ব্যাচ-২ |
| 7 | Creatine for Women | ইন্ট্রো প্যারাগ্রাফ + TOC নেই | ⏳ ব্যাচ-৩ |
| 8 | Lower Cortisol | ইন্ট্রো প্যারাগ্রাফ + TOC নেই | ⏳ ব্যাচ-৩ |
| 9 | Magnesium Foods | ইন্ট্রো প্যারাগ্রাফ + TOC নেই | ⏳ ব্যাচ-৩ |
| 10 | Mobility Hips | ইন্ট্রো প্যারাগ্রাফ + TOC নেই | ⏳ ব্যাচ-৩ |
| 11 | Protein Moment | ইন্ট্রো প্যারাগ্রাফ + TOC নেই | ⏳ ব্যাচ-৩ |
| 12 | Grip Strength | ইন্ট্রো প্যারাগ্রাফ + TOC নেই | ⏳ ব্যাচ-৩ |
| 13 | Anti-Inflammatory | ইন্ট্রো প্যারাগ্রাফ + TOC নেই | ⏳ ব্যাচ-৩ |
| 14 | Evening Routine | ইন্ট্রো প্যারাগ্রাফ + TOC নেই | ⏳ ব্যাচ-৩ |
| 15 | Best Foods Gut Health | SEO ব্রিফ কমেন্ট | ⏳ ব্যাচ-৪ |
| 16 | High Fiber (and gut) | SEO ব্রিফ কমেন্ট | ⏳ ব্যাচ-৪ (রাখুন) |
| 17 | High Fiber (that work) | SEO ব্রিফ কমেন্ট + **ডুপ্লিকেট** | ⏳ ব্যাচ-৪ (রিডাইরেক্ট/রি-রাইট) |
| 18 | Lose Weight Fast | SEO ব্রিফ কমেন্ট + স্লাগ স্যাফিক্স | ⏳ ব্যাচ-৪ |
| 19 | 9 Foods Blood Pressure | SEO ব্রিফ কমেন্ট | ⏳ ব্যাচ-৪ |
| 20 | Fibermaxxing | ইমেজ প্রথমে নেই, টেমপ্লেট ভিন্ন | ⏳ ব্যাচ-৫ |
| 21 | Sleep Hygiene | ইমেজ প্রথমে নেই | ⏳ ব্যাচ-৫ |
| 22 | Fix Sleep Schedule | ইমেজ প্রথমে নেই | ⏳ ব্যাচ-৫ |
| 23 | Heart-Healthy Eating | ইমেজ প্রথমে নেই | ⏳ ব্যাচ-৫ |
| 24 | Japanese Walking | `<style>` + ব্যানার কমেন্ট | ⏳ ব্যাচ-৬ |
| 25 | Morning Routine | `<style>` + ব্যানার কমেন্ট | ⏳ ব্যাচ-৬ |
| 26 | One Weekly Walk | `<style>` + ব্যানার কমেন্ট | ⏳ ব্যাচ-৬ |
| 27 | 7-Day Meal Plan | ইমেজ প্রথমে নেই | ⏳ ব্যাচ-৫ |
| 28 | 10 Evidence Tips | `body {}` গ্লোবাল সিএসএস | ⏳ ব্যাচ-৬ (ক্রিটিক্যাল) |
| 29 | Post-Meal Walking | `body {}` গ্লোবাল সিএসএস | ⏳ ব্যাচ-৬ (ক্রিটিক্যাল) |
| 30 | Strength Training | `body {}` গ্লোবাল সিএসএস | ⏳ ব্যাচ-৬ (ক্রিটিক্যাল) |
| 31 | Mental Health | স্কোপড সিএসএস + খারাপ স্লাগ | ⏳ ব্যাচ-৬ |
| 32 | Retatrutide Lawsuits | স্কোপড সিএসএস + খারাপ স্লাগ | ⏳ ব্যাচ-৬ |
| 33 | Fitness Trackers | স্কোপড সিএসএস | ⏳ ব্যাচ-৬ |
| 34 | Candida auris | `html,body {}` + `!important` | ⏳ ব্যাচ-৬ (ক্রিটিক্যাল) |

---

## ফিক্স করার নিয়ম (প্রতিটি পোস্টে একই প্যাটার্ন — "গোল্ড স্ট্যান্ডার্ড")

সব ফিক্সড ফাইল এই ক্রম মেনে তৈরি হচ্ছে (থিম v19-এর ক্লাস ব্যবহার করে):

1. **ফিচার্ড ইমেজ** — `<img>` with descriptive alt, `border-radius:12px` স্টাইল, প্রথমে
2. **ইন্ট্রো প্যারাগ্রাফ** — ১–৩টি `<p>`, সম্ভব হলে ১–২টি ইন্টারনাল লিংকসহ
3. **টেবিল অফ কন্টেন্ট** — `<details class="toc toc-slim">` (কলাপ্সড), প্রতিটি `<h2>`-এর `id`-এর সাথে মিলিয়ে
4. **Key Takeaways** — `<div class="key-takeaways">`
5. **মূল আর্টিকেল** — `<h2 id="...">` সেকশন; টেবিল হলে `<div class="vtd-table-wrap">`; সতর্কতা হলে `<div class="warning-box">`
6. **FAQ** — `<details class="faq-item">`
7. **সোর্স বক্স** — `<div class="source-box" id="references">` (NIH/CDC/PubMed/DOI লিংক, `rel="nofollow noopener"`)
8. **মেডিক্যাল ডিসক্লেইমার** — `<div class="medical-disclaimer">` (সবার শেষে)

**মুছে ফেলা হয়:** সব `<style>` ব্লক, ইনজেক্টেড `<script>`, SEO ব্রিফ কমেন্ট, ব্যানার কমেন্ট, অপ্রয়োজনীয় র‍্যাপার ডিভ ও ইনলাইন স্টাইল।

---

## ইন্টারনাল লিংক ম্যাপ (ক্যানোনিক্যাল — সব ভবিষ্যৎ ফিক্সে এগুলোই ব্যবহার হবে)

সব ইন্টারনাল লিংক এই ৩৪টি লাইভ URL-এর মধ্যেই হতে হবে (ভাঙা লিংক এড়াতে):
```
/2026/09/circadian-rhythm-reset-how-aligning.html
/2026/09/berberine-explained-is-natures-ozempic.html
/2026/09/how-to-build-healthy-plate-for-stable.html
/2026/09/natural-glp-1-foods-12-science-backed.html
/2026/09/cortisol-belly-how-to-lose-7-day-plan.html
/2026/09/alcohol-cancer-deaths-double-in-america.html
/2026/09/creatine-for-women-benefits-dosage-and.html
/2026/09/how-to-lower-cortisol-naturally-8.html
/2026/09/magnesium-rich-foods-for-muscle-recovery.html
/2026/08/mobility-exercises-for-stiff-hips-that.html
/2026/08/why-protein-is-having-moment-how-much.html
/2026/08/why-grip-strength-may-predict-how-long.html
/2026/08/anti-inflammatory-foods-for-joint.html
/2026/08/evening-routine-for-better-sleep-that.html
/2026/08/best-foods-for-gut-health-and-digestion.html
/2026/08/high-fiber-foods-for-digestion-and-gut.html
/2026/08/high-fiber-foods-for-digestion-that.html
/2026/08/how-to-lose-weight-fast-naturally_0802718094.html
/2026/08/9-foods-for-high-blood-pressure-that.html
/2026/08/fibermaxxing-explained-how-much-fiber.html
/2026/08/science-backed-sleep-hygiene-tips-for.html
/2026/08/how-to-fix-your-sleep-schedule.html
/2026/08/heart-healthy-eating-plan-for-beginners.html
/2026/08/japanese-walking-30-minute-science.html
/2026/08/morning-routine-for-energy-7-habits.html
/2026/08/one-weekly-walk-cuts-belly-fat-as-well.html
/2026/08/7-day-healthy-and-balanced-meal-plan.html
/2026/08/10-evidence-based-health-tips-every.html
/2026/08/walking-after-meals-blood-sugar-research.html
/2026/08/strength-training-for-beginners-safe.html
/2026/08/a-person-sitting-calmly-outdoors-in.html
/2026/08/wooden-gavel-beside-prescription.html
/2026/08/top-benefits-of-fitness-trackers-for.html
/2026/08/candida-auris-prevention-how-strong.html
```
(বেস: `https://vitaltipsdaily.blogspot.com`)

এখন পর্যন্ত চেক করা ইন্টারনাল লিংকগুলো (Circadian, Berberine, Healthy Plate পোস্টে) সব ভ্যালিড — ৪০৪ পাওয়া যায়নি।

---

## থিম নিয়ে নোট

`vitaltipsdaily-theme-seo-fixed-v19.xml` ফাইলটি আপলোড থেকে আমার ওয়ার্কস্পেসে পৌঁছায়নি (সিঙ্ক ব্যর্থ)। লাইভ সাইট রেন্ডার থেকে যা দেখা গেছে:
- থিমটি `toc`, `toc-slim`, `key-takeaways`, `warning-box`, `source-box`, `medical-disclaimer`, `faq-item`, `vtd-table-wrap` ক্লাসগুলো স্টাইল করে (Circadian পোস্টে সুন্দরভাবে রেন্ডার হচ্ছে)
- তাই ফিক্সড ফাইলগুলো ইনলাইন সিএসএসের বদলে এই থিম-ক্লাস ব্যবহার করে

**অনুরোধ:** থিম ফাইলটি আবার অ্যাটাচ করুন — থিমের `<head>` সেকশন (মেটা ট্যাগ, স্কিমা, সোশ্যাল লিংক) আলাদাভাবে অডিট করে দেব।

---

## কীভাবে অ্যাপ্লাই করবেন (প্রতিটি ফিক্সড ফাইলের জন্য)

1. ফাইলটি খুলুন (উপরের `<!-- FIXED ... -->` কমেন্ট লাইনটি মুছে ফেলুন)
2. Blogger → পোস্ট → **HTML view**-তে যান
3. পুরনো সব কোড মুছে নতুন কোড পেস্ট করুন
4. **Search Description** ঘরে ১৫০–১৬০ অক্ষরের মেটা ডেসক্রিপশন দিন
5. পোস্ট সেটিংসে **Labels** ঠিক রাখুন
6. আপডেট/পাবলিশ করুন
