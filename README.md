# 🤖 JARVIS v2.0 — SUPER SMART EDITION

Iron Man ke Jarvis jaisa **super-intelligent** voice assistant!

## 🧠 Kya-kya SUPER POWERS hain

### 1. Function Calling (Agentic AI) 🔥
Gemini sirf text nahi bolta — **khud tools call karta hai!**
```
Tum: "Mummy ko 5 baje call karne ka reminder lagao aur WhatsApp kholo"
Jarvis: [schedule_reminder call] + [open_app call] → "Ho gaya! ✅"
```
Multi-step tasks **khud plan karke** execute karta hai!

### 2. Vision — Screenshot dekh ke samajhta hai 👁️
- Complex apps (Zomato, Flipkart) me screenshot leke Gemini Vision se puchta hai
- "Kahan tap karun?" — coordinates ke saath jawab!

### 3. Self-Healing Macros 🎬
- Step fail ho to **khud fix karta hai** — 3 attempts, smart strategies
- Text nahi mila? Screen dobara scan → milta-julta button → scroll karke dhoondho
- Report batata hai: "2 steps khud fix kiye!"

### 4. Routine Learning 📊
- Tumhare patterns seekhta hai: "Roz subah 9 baje Zomato kholte ho"
- 3 baar repeat = permanent routine memory!

### 5. Proactive Engine 💡
- Bina puche sahi time pe suggest karta hai
- "Roz is time chai order karte ho, kar dun?"
- Pending reminders + time-based nudges

### 6. Smart Memory (slow nahi hota!) 💾
- Sirf 1-line summaries, poori chat kabhi context me nahi
- Importance + usage se ranking
- Bekar memories auto-delete

### 7. Wake Word 🎤 — "Hey Jarvis" (FREE, koi account nahi!)
- openWakeWord ka pre-trained AI model — phone me hi chalta hai
- **Koi signup nahi, koi API key nahi, koi company email nahi!**
- 100% offline — tumhari awaz phone se bahar nahi jati
- Models app ke andar bundled hain (~3.7MB)

### 8. Editable Prompt ✏️
- Jarvis ka dimaag tum edit kar sakte ho
- Ya bolo "apna prompt badlo"

## 🗣️ Example Commands

```
"Zomato kholo aur biryani search karo"
"Mummy ko 5 baje call karne ka reminder lagao"
"Yaad rakho meri chai me cheeni kam"
"Macro record karo morning routine" → steps karo → "macro save karo"
"Macro chalao morning routine"
"Screen pe kya hai?"
"Hey Jarvis" (wake word)
```

## 🔧 Setup

### 1. Gemini API Key (FREE)
https://aistudio.google.com → Get API Key → App Settings me paste karo

### 2. Accessibility ON karo
App me "♿ Screen Control" → Jarvis → Enable

### 3. Wake Word — kuch karna hi nahi! 🎤
- App kholte hi **"Hey Jarvis"** sunna shuru kar deta hai
- Bolo "Hey Jarvis" → wo puchega "Haan?" → apna command bolo!
- Bilkul free, offline, koi account nahi chahiye

### 4. Daily Briefing
Settings → "Roz subah 8 baje briefing ON karo"

## 🏗️ Build

**Android Studio:** Open folder → Sync → Run ▶️

```bash
./gradlew assembleDebug
# APK: app/build/outputs/apk/debug/app-debug.apk
```

## 📁 Architecture

```
JarvisBrain.kt           # 🧠 Agentic brain (function calling loop)
SmartGeminiClient.kt     # Gemini + tools + vision API
GeminiFunctions.kt       # 9 tools: reminder, app, tap, type, scroll, macro...
VisionHelper.kt          # Screenshot → Gemini Vision
SelfHealingMacro.kt      # Auto-fix macro executor
RoutineLearner.kt        # Pattern detection
ProactiveEngine.kt       # Smart suggestions
MemoryManager.kt         # Smart summaries (never slow)
MacroManager.kt          # Record/play macros
TaskScheduler.kt         # Alarms + daily briefing
WakeWordManager.kt       # "Hey Jarvis" detection
VoiceManager.kt          # Hindi TTS + speech recognition
JarvisAccessibilityService.kt  # Screen control
```

## 🔐 Privacy
- Saara data **phone me** (Room DB)
- Gemini ko sirf command + relevant memories jaati hain
- Koi tracking nahi

## ⚠️ Important Notes
- **Payment steps** (UPI PIN) kabhi macro me record mat karo
- Flipkart/Zomato **order place** karne se pehle hamesha confirm karega
- Accessibility permission sirf tumhare commands pe kaam karti hai

---

**Ab tumhara phone sach me Jarvis jaisa! 🚀🔥**
