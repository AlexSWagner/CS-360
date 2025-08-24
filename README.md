# XelaPlanner - Android Event Management Application

This repository contains the source code for **XelaPlanner**, a native Android application developed as a course project. The app is a modern, user-centric event and schedule management tool built with **Kotlin** and **Jetpack Compose**, following the latest Android development best practices.

---

## Project Summary and User Needs
The primary goal of XelaPlanner was to develop a robust and intuitive application for tracking upcoming events.  
The app was designed for busy individuals who need a powerful yet simple tool to manage their schedules.  

Through user persona development, I identified three key user groups:
- **Diligent Student**
- **Busy Professional**
- **Busy Parent**

The core user need for all three groups was:
- A clear, reliable, and fast way to see their schedule  
- Manage events with minimal friction  
- Receive timely reminders  

---

## User-Centered UI Design
To support these user needs, I built the application around a **two-part Event Dashboard**:
- An interactive **monthly calendar** for a high-level overview  
- A **dynamic agenda** for detailed planning  

This allows users to seamlessly switch between "big picture" and focused daily views.  

Key UI design choices:
- Instead of a disruptive FloatingActionButton, a prominent **"+ Add Event"** button was integrated directly into the agenda header.  
- **Single tap** on an event card → opens edit form  
- **Long-press** on an event card → triggers delete confirmation  

This interaction model is intuitive and keeps the interface uncluttered.

---

## Development Approach and Strategy
The application was developed using:
- **Jetpack Compose** for UI  
- **MVVM architecture** for state management  
- **Unidirectional Data Flow (UDF)** principles  

This approach ensures:
- Clear separation of concerns  
- Easier debugging, maintenance, and testing  
- A scalable structure I plan to apply in future projects  

---

## Testing and Functionality
To ensure functionality, I used an **iterative testing strategy**:
- Built a **state-driven UI** using mock data in the ViewModel  
- Fully developed and tested the UI—including **animations** and **filtering**—before implementing the database backend  
- Iteratively tested each change on an Android Virtual Device (AVD)  

This process isolated the UI layer for rapid iteration and helped identify early UX flaws.

---

## Innovation and Overcoming Challenges
One major challenge was handling **multiple user actions** on a single UI element without cluttering the interface.  

Solution: **Dual-action gesture system** on the calendar view:  
- **Single tap** on a day → filters the agenda  
- **Long-press** on a day → initiates the "add event" flow  

This provided both primary and secondary actions elegantly without adding extra buttons.

---

## Demonstration of Skills
The **Event Dashboard** is the highlight of the project. It demonstrates advanced Android development skills by combining:
- A **custom calendar grid**  
- A **dynamic LazyColumn**  
- **Reactive state management** with ViewModel + StateFlow  
- An **intuitive gesture-based interaction model**  

The final result is a polished, professional-grade interface that translates user needs into a seamless experience.

---
