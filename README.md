# 📝 Junior Frontend Developer Challenge

**Project Title:** Offline‑Capable Notes App with Conflict Resolution  
**Stack:** Angular 17+ (Standalone Components), @ngrx/signals, Firebase (Auth + Firestore)

---

## 1. 🔍 Overview

Build a feature-rich notes application that works offline, syncs with Firebase Firestore, and intelligently handles conflicts. This challenge evaluates your skills in:

- Angular 17+ with standalone components  
- State management with `@ngrx/signals` (Signal Store)  
- Firebase integration (Auth, Firestore, offline persistence)  

---

## 2. 🎯 Objectives

Your app must allow users to:
1. Sign in **anonymously** using Firebase Auth  
2. Perform CRUD on notes (title + content)  
3. Add, edit, and delete notes **offline**  
4. Automatically sync with Firestore when back online  
6. Manage all state with `@ngrx/signals`

---

## 3. ⚙️ Requirements

### Angular Setup
- Use **Angular 17+**
- Use **standalone components**

### State Management
- Use `@ngrx/signals` or **Signal Store**
- Store all notes, sync status, conflict states in Signals

### Firebase Integration
- Use modular Firebase SDK v10+
- Enable Firestore **offline persistence**
- Note document shape:
  ```ts
  type Note = {
    id: string;
    title: string;
    content: string;
    updatedAt: Timestamp;
    version: number; // incremented each write
  };

---

## 4. 💡 Optional Bonuses:
- Simple CRDT-like merging (e.g., combining non-overlapping edits)
- LocalStorage cache for faster loads
- Undo/Redo via signal actions

---

## 5. 📁 Deliverables:
- GitHub repo/ZIP with full Angular project
- README.md with:
- Setup instructions
- How to simulate offline & conflict scenarios
- Well-structured code (components, stores, services)

---

## 6. ✅ Evaluation Criteria:
| Criteria                                 | Weight          |
|-----------------------------------------|-----------------|
| Offline‑first UI & Firestore sync       | ⭐⭐⭐⭐           |
| Conflict resolution UI & logic          | ⭐⭐⭐⭐           |
| Proper use of `@ngrx/signals`          | ⭐⭐⭐⭐           |
| Code readability & modularity           | ⭐⭐⭐            |
| Bonus features (merge, undo/redo, presence) | ⭐⭐        |

---
## Good luck! 🎉

We look forward to seeing your skills in action.
