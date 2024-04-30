Foodium 🍲 
Test Build Lint

GitHub license Android Weekly ktlint Github Followers GitHub stars GitHub forks GitHub watchers Twitter Follow

Foodium is a sample food blog 🍲 Android application 📱 built to demonstrate use of Modern Android development tools. Dedicated to all Android Developers with ❤️.

You can Install and test latest Foodium app from below 👇

Foodium App

About
It simply loads Posts data from API and stores it in persistence storage (i.e. SQLite Database). Posts will be always loaded from local database. Remote data (from API) and Local data is always synchronized.

This makes it offline capable 😃.
Clean and Simple Material UI.
It supports dark theme too 🌗.
Dummy API is used in this app. JSON response is statically hosted here.

Built With 🛠
Kotlin - First class and official programming language for Android development.
Coroutines - For asynchronous and more..
Flow - A cold asynchronous data stream that sequentially emits values and completes normally or with an exception.
Android Architecture Components - Collection of libraries that help you design robust, testable, and maintainable apps.
LiveData - Data objects that notify views when the underlying database changes.
ViewModel - Stores UI-related data that isn't destroyed on UI changes.
ViewBinding - Generates a binding class for each XML layout file present in that module and allows you to more easily write code that interacts with views.
Room - SQLite object mapping library.
Dependency Injection -
Hilt-Dagger - Standard library to incorporate Dagger dependency injection into an Android application.
Hilt-ViewModel - DI for injecting ViewModel.
Retrofit - A type-safe HTTP client for Android and Java.
Moshi - A modern JSON library for Kotlin and Java.
Moshi Converter - A Converter which uses Moshi for serialization to and from JSON.
Coil-kt - An image loading library for Android backed by Kotlin Coroutines.
Material Components for Android - Modular and customizable Material Design UI components for Android.
Gradle Kotlin DSL - For writing Gradle build scripts using Kotlin.
Lint ✅
This project uses GitHub Super Linter which is Combination of multiple linters to install as a GitHub Action.

Following Linters are used internally by super linter (enabled for this project):

XML: LibXML
Kotlin: ktlint
Dagger (Old) DI Version 🗡️
If you want to refer old way of Dependency Injetion using Dagger2, see branch dagger2-di

Dagger2 Version

Koin DI Version 🗡️
If you want to use Koin - Dependency Injection framework in app then visit below repository.

Koin Version

Contributed By: Pranay Patel

Package Structure
dev.shreyaspatil.foodium    # Root Package
.
├── data                # For data handling.
│   ├── local           # Local Persistence Database. Room (SQLite) database
|   │   ├── dao         # Data Access Object for Room   
│   ├── remote          # Remote Data Handlers     
|   │   ├── api         # Retrofit API for remote end point.
│   └── repository      # Single source of data.
|
├── model               # Model classes
|
├── di                  # Dependency Injection             
│   ├── builder         # Activity Builder
│   ├── component       # DI Components       
│   └── module          # DI Modules
|
├── ui                  # Activity/View layer
│   ├── base            # Base View
│   ├── main            # Main Screen Activity & ViewModel
|   │   ├── adapter     # Adapter for RecyclerView
|   │   └── viewmodel   # ViewHolder for RecyclerView   
│   └── details         # Detail Screen Activity and ViewModel
|
└── utils               # Utility Classes / Kotlin extensions
Architecture
This app uses MVVM (Model View View-Model) architecture.



Contribute
If you want to contribute to this library, you're always welcome! See Contributing Guidelines.

Discuss 💬
Have any questions, doubts or want to present your opinions, views? You're always welcome. You can start discussions.

Contact
