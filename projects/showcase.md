# 📁 Project Showcase — Piyush

> Deep-dive writeups for each repository. For the quick-scan overview, see the [main README](../README.md).

---

## Table of Contents

- [MoodNest — iOS Mood Tracker](#-moodnest--ios-mood-tracker)
- [ToDoApp — iOS Productivity](#-todoapp--ios-productivity)
- [Nectar — iOS App](#-nectar--ios-app)
- [PatsApp — iOS Messaging & Community](#-patsapp--ios-messaging--community)
- [Grocery List — iOS Grocery Manager](#-grocery-list--ios-grocery-manager)
- [bling-redteam — AI Security / Red Teaming](#-bling-redteam--ai-security--red-teaming)

---

## 🧠 MoodNest — iOS Mood Tracker

![Swift](https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0070C9?style=for-the-badge&logo=swift&logoColor=white)
[![Repo](https://img.shields.io/badge/GitHub-161b22?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Piyush-072006-B/MoodNest-7.2F2)

### What It Is

MoodNest is a mental wellness companion for iOS, built entirely in Swift and SwiftUI. It gives users a private, friction-free space to log how they're feeling each day — and over time, helps them see patterns in their emotional landscape.

Mental health apps often either feel clinical and cold, or try to be so cute they become annoying. MoodNest aims to be neither — just a quiet, honest tool that respects the user's time and emotional intelligence.

### Core Features

| Feature | Description |
|---------|-------------|
| **Daily Mood Logging** | Log your mood in seconds with an intuitive input — no lengthy forms |
| **Pattern Visualization** | Charts and graphs that reveal emotional trends over days and weeks |
| **Private by Design** | All data stored locally on device — no account needed, no cloud sync |
| **Journal Integration** | Optional freeform notes to add context to each mood entry |
| **Streak Tracking** | Gentle nudges to keep consistent without being pushy |

### Technical Highlights

- **SwiftUI** for the entire UI layer — fully declarative, responsive across all iPhone screen sizes
- **Swift Charts** (or Core Graphics) for visualizing mood trends
- **UserDefaults / Core Data** for persistent local storage
- Clean MVVM architecture separating view logic from data models
- Custom UI components built from scratch — no third-party UI libraries

### What I Learned

Building MoodNest pushed me to think seriously about UX design — specifically, how small UI decisions (animation speed, color choice, tap target size) affect how an app *feels* during vulnerable moments. I learned that wellness apps need to be calm by design, not just by color palette.

---

## ✅ ToDoApp — iOS Productivity

![Swift](https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0070C9?style=for-the-badge&logo=swift&logoColor=white)
[![Repo](https://img.shields.io/badge/GitHub-161b22?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Piyush-072006-B/ToDoApp)

### What It Is

A fast, clean task management app for iPhone. ToDoApp was built with a specific philosophy: **zero friction between thought and action**. If it takes more than 2 taps to add a task, the app has failed.

This project was an exercise in restraint. The challenge wasn't adding features — it was deciding what *not* to add.

### Core Features

| Feature | Description |
|---------|-------------|
| **Instant Task Creation** | Tap once, type, done. Tasks are created instantly with no modal friction |
| **Priority Tagging** | Mark tasks as high / medium / low priority at a glance |
| **Swipe Actions** | Swipe to complete or delete — native iOS gestures, not custom workarounds |
| **Persistent Storage** | Tasks survive app restarts — nothing is ever lost |
| **Clean List View** | No cluttered sidebars, no subscription prompts, just your tasks |

### Technical Highlights

- Pure **SwiftUI** with `@State`, `@Binding`, and `@ObservedObject` for reactive data flow
- **Core Data** integration for persistent, reliable local storage
- Native `List` with custom swipe actions and delete confirmations
- MVVM pattern — ViewModel handles all business logic, Views stay thin

### What I Learned

This was my first serious exercise in data persistence in iOS. Getting Core Data to play nicely with SwiftUI required understanding the `@Environment(\.managedObjectContext)` pattern, and debugging crashes related to threading taught me a lot about how Core Data manages its context stack.

---

## 🌸 Nectar — iOS App

![Swift](https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=apple&logoColor=white)
[![Repo](https://img.shields.io/badge/GitHub-161b22?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Piyush-072006-B/Nectar)

### What It Is

Nectar is an iOS app with a strong emphasis on fluid motion and polished interface design. The name evokes something smooth, rich, and desirable — and that's the standard the app's UX is held to.

This project was primarily a design-driven build: start with how it *feels*, then figure out the architecture. It's an exploration of what SwiftUI can do when you push its animation system hard.

### Core Features

| Feature | Description |
|---------|-------------|
| **Fluid Animations** | Every transition is choreographed — nothing jerks or pops |
| **Custom Navigation** | Hand-rolled navigation patterns that go beyond standard NavigationView |
| **Polished Micro-interactions** | Taps, swipes, and gestures all have satisfying feedback |
| **Visual Hierarchy** | Typography and spacing tuned for effortless scanning |

### Technical Highlights

- Heavy use of SwiftUI's `.animation()` and `withAnimation()` APIs
- Custom `matchedGeometryEffect` for hero-style shared element transitions
- `GeometryReader` for responsive, context-aware layout
- Focus on `@Namespace` and view identity for smooth state transitions

### What I Learned

Nectar taught me that animation is about timing and easing curves, not just movement. I spent significant time tweaking spring parameters to get that "expensive app" feel — the difference between `easeInOut` and a well-tuned spring response is enormous in perceived quality.

---

## 🐾 PatsApp — iOS Messaging & Community

![Swift](https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0070C9?style=for-the-badge&logo=swift&logoColor=white)
[![Repo](https://img.shields.io/badge/GitHub-161b22?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Piyush-072006-B/PatsApp)

### What It Is

PatsApp is a community and messaging iOS app built around pets. Share photos of your animals, connect with other pet owners, and message within a purpose-built community — all in a native Swift app. It's niche by design: focused community apps win where general social networks lose.

### Core Features

| Feature | Description |
|---------|-------------|
| **Real-time Messaging** | Send and receive messages natively in Swift |
| **Pet Profiles** | Create profiles for your pets — not just yourself |
| **Community Feed** | Browse and share pet moments with the community |
| **Photo Sharing** | Native iOS photo picker integration |
| **Notifications** | Push notifications for messages and community activity |

### Technical Highlights

- **Real-time messaging** architecture — WebSockets or Firebase Realtime Database
- **Photo Library integration** using `PhotosUI` framework (`PHPickerViewController`)
- Complex SwiftUI view hierarchy managing multiple screens and navigation stacks
- Async/await for network calls — modern Swift concurrency patterns
- Push notification setup via APNs (Apple Push Notification service)

### What I Learned

PatsApp was my most ambitious project in terms of feature scope. Managing real-time state across a messaging interface — handling optimistic updates, delivery receipts, and error states — is genuinely hard. It pushed me deep into Swift concurrency and async data flows.

---

## 🛒 Grocery List — iOS Grocery Manager

![Swift](https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=apple&logoColor=white)
[![Repo](https://img.shields.io/badge/GitHub-161b22?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Piyush-072006-B/Grocery-List)

### What It Is

A grocery management app that solves a real, everyday problem: the chaos of the supermarket. Organize items by aisle category, check things off as you shop, and never leave the store without everything on the list.

This project was about shipping something genuinely useful. Not impressive from a technical complexity standpoint, but solid, reliable, and something people would actually use.

### Core Features

| Feature | Description |
|---------|-------------|
| **Category Organization** | Items grouped by category (Produce, Dairy, Frozen, etc.) |
| **Check-off UX** | Tap to check items off with a satisfying strikethrough animation |
| **Quick Add** | Add items rapidly with an autocomplete-style input |
| **List Management** | Create multiple lists (weekly shop, party supplies, etc.) |
| **Share List** | Share your list with family members for collaborative shopping |

### Technical Highlights

- `List` with grouped sections using SwiftUI's `ForEach` + `Section` pattern
- Custom animations on item completion states
- Enum-based category system with associated display properties
- **ShareLink** API for native list sharing
- `@AppStorage` for lightweight preference persistence

### What I Learned

Building a "simple" app exposed how much thought goes into data modeling. Choosing the right data structure for categorized, ordered lists — and keeping it performant when lists grow large — was more nuanced than I expected. Simplicity in UX requires complexity in thinking.

---

## 🛡️ bling-redteam — AI Security / Red Teaming

![Python](https://img.shields.io/badge/Python-3572A5?style=for-the-badge&logo=python&logoColor=white)
![AI Security](https://img.shields.io/badge/AI_Security-7c3aed?style=for-the-badge&logo=shieldsdotio&logoColor=white)
![Red Teaming](https://img.shields.io/badge/Red_Teaming-9333ea?style=for-the-badge&logo=hackaday&logoColor=white)
[![Repo](https://img.shields.io/badge/GitHub-161b22?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Piyush-072006-B/bling-redteam)

### What It Is

`bling-redteam` is a Python project focused on AI red teaming — the practice of adversarially testing large language models to expose their failure modes, safety gaps, and unexpected behaviors.

This is where my AI/ML curiosity intersects with security thinking. Red teaming LLMs is a serious, emerging discipline at the frontier of AI safety research. For a first-year student to be poking at it means thinking several steps ahead of the typical CS curriculum.

### What Red Teaming Means

AI red teaming involves:
- **Adversarial prompting**: Crafting inputs designed to elicit unsafe, incorrect, or unintended model outputs
- **Jailbreak exploration**: Testing whether safety guardrails can be bypassed via prompt engineering
- **Bias probing**: Identifying systematic skews in model responses across demographic or topical dimensions
- **Robustness testing**: Checking whether small input variations cause large, unexpected output changes

### Core Areas Explored

| Area | Description |
|------|-------------|
| **Prompt Injection** | Techniques to override model instructions via crafted user inputs |
| **Jailbreak Patterns** | Systematic cataloguing of prompt patterns that bypass safety filters |
| **Adversarial Examples** | Inputs specifically crafted to cause model misbehavior |
| **Evaluation Pipelines** | Python tooling to run, log, and analyze large batches of red-team prompts |

### Technical Highlights

- Python scripting with LLM API integrations (OpenAI, Anthropic, or local models)
- Automated batch testing of prompt variations across multiple model configurations
- Structured logging and output analysis for pattern identification
- Probabilistic evaluation of model response safety and coherence

### Why This Matters

AI systems are being deployed in healthcare, finance, legal, and education. Understanding their failure modes isn't optional — it's essential. Projects like `bling-redteam` are how you learn to build AI systems that are genuinely trustworthy, not just superficially safe.

> "If you can't break it, you don't understand it."

---

<p align="center">
  <a href="../README.md">← Back to Profile</a>
</p>
