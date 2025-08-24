# XelaPlanner - Android Event Management Application

This repository contains the source code for XelaPlanner, a native Android application developed as a course project. The app is a modern, user-centric event and schedule management tool built with Kotlin and Jetpack Compose, following the latest Android development best practices.

## Project Summary and User Needs

The primary goal of XelaPlanner was to develop a robust and intuitive application for tracking upcoming events. The app was designed for busy individuals who need a powerful yet simple tool to manage their schedules. Through user persona development, I identified three key user groups: the Diligent Student, the Busy Professional, and the Busy Parent. The core user need for all three groups was a clear, reliable, and fast way to see their schedule, manage events with minimal friction, and receive timely reminders.

## User-Centered UI Design

To support these user needs, I built the application around a sophisticated, two-part Event Dashboard. This screen features an interactive monthly calendar for a high-level overview and a dynamic agenda for detailed planning, allowing users to seamlessly switch between "big picture" and focused daily views.

The UI was designed with the user in mind at every step. Instead of a disruptive FloatingActionButton, a prominent "+ Add Event" button was integrated directly into the agenda header. The interaction model was refined through an iterative process: a single tap on an event card opens the edit form, while a long-press triggers a delete confirmation. This workflow is more intuitive and efficient than cluttering the UI with persistent icons.

## Development Approach and Strategy

I developed the application using a modern technology stack centered on Jetpack Compose for the UI and a Model-View-ViewModel (MVVM) architecture for state management. This approach follows the principle of a Unidirectional Data Flow (UDF), where the UI is a direct function of its state. This strategy is highly effective as it creates a clear separation of concerns, making the code significantly easier to debug, maintain, and test. I will apply this technique of decoupling the UI from the logic to all my future projects.

## Testing and Functionality

To ensure the code was functional, I used an iterative testing strategy. I initially built the application with a state-driven UI using mock data in the ViewModel. This allowed me to fully develop and test the interactive UI—including animations and filtering—without needing a fully implemented database backend. This process is important because it isolates the UI layer for rapid iteration and revealed several initial UX flaws that I was then able to correct. Every small change was followed by running the app on an Android Virtual Device (AVD) to ensure stability.

## Innovation and Overcoming Challenges

A significant challenge was how to handle multiple user actions on a single UI element without creating a cluttered interface. My innovative solution was to implement a dual-action gesture system on the calendar view. A single tap on a day filters the agenda, while a long-press initiates the "add event" flow for that specific date. This approach solved the UX conflict elegantly, providing both primary and secondary actions on a single component without adding extra buttons to the UI.

## Demonstration of Skills

I was particularly successful in demonstrating my knowledge and skills in the implementation of the main Event Dashboard. This single screen is a complex, state-driven component that showcases a professional understanding of modern Android development. It effectively combines a custom calendar grid, a dynamic LazyColumn, reactive state management with a ViewModel and StateFlow, and an intuitive, gesture-based interaction model. The final result is a seamless and highly usable interface that successfully translates the initial user needs into a polished final product.
