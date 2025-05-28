# Valoro.MAUI - Blazor Hybrid App (.NET 9)

Valoro.MAUI is a cross-platform mobile and desktop app for financial currency exchange built using .NET MAUI and Blazor Hybrid technology. It enables the use of Blazor components and Razor pages within a native app via a BlazorWebView control.

---

## 📱 Project Overview

This project is part of the Valoro suite, a .NET 9 solution with:

- `Valoro.Web.Client`: Blazor WebAssembly frontend
- `Valoro.Web`: ASP.NET Core Host + API backend
- `Valoro.MAUI`: Blazor Hybrid App (mobile/desktop)
- `Valoro.Shared`: Shared models and services

---

## 🧠 Key Features

- Uses **BlazorWebView** to render interactive Razor components inside native apps.
- Supports navigation via **Shell** (`AppShell.xaml`) for modern routing.
- Communicates with backend API using `HttpClient` via dependency injection.
- Shares logic and models via `Valoro.Shared`.

---

## 🛠️ Project Structure

```
Valoro.MAUI/
├── App.xaml
├── App.xaml.cs        # Entry point of the application
├── AppShell.xaml      # Shell navigation structure
├── AppShell.xaml.cs
├── MainPage.xaml      # Hosts BlazorWebView
├── MainPage.xaml.cs
├── wwwroot/           # Contains index.html for BlazorWebView
└── MauiProgram.cs     # DI configuration and Blazor setup
```

---

## 🚀 Getting Started

1. **Build the solution** in Visual Studio 2022+ with .NET 9 SDK installed.
2. Set **Valoro.MAUI** as the startup project.
3. Run on Android emulator, iOS simulator, or Windows/Mac desktop.

---

## 🌐 API Connectivity

Valoro.MAUI communicates with the backend API (`Valoro.Web` or `Valoro.API`) through a configured `HttpClient`. Ensure CORS is properly set up on the backend.

---

## 🔄 Shared Code

`Valoro.Shared` contains all reusable DTOs, interfaces, and services consumed by both the Web and MAUI apps.

---

## 💡 Notes

- Ensure platform-specific permissions are set for network access.
- Blazor components used here are fully reusable with `Valoro.Web.Client`.

