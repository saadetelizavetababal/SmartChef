# SmartChef

## 📖 Description

**SmartChef** is an intelligent, cross-platform meal assistant designed to make cooking easier, smarter, and more personalized.  
The project consists of both a **responsive web application** and a **cross-platform mobile application**, built using modern frameworks and connected via a shared backend API.  

At its core, SmartChef leverages **Artificial Intelligence (AI)** and real-time **data-driven APIs** to provide users with personalized recipe recommendations based on the ingredients they already have at home.  
Users can input available ingredients manually or via image recognition (mobile), and SmartChef's AI module matches them with suitable recipes by analyzing ingredient compatibility, nutritional data, and user preferences.

The system also supports a **meal planner**, allowing users to organize their meals across the week, as well as save favorite recipes and receive smart suggestions based on past selections.

SmartChef aims to reduce food waste, simplify home cooking, and encourage healthier eating habits with the power of technology.

---

### 🧠 AI & API Highlights

- 🔍 **AI-Powered Recipe Recommendation:**  
  Uses NLP and ingredient vector similarity to match recipes with user-input ingredients.
  
- 📦 **API Integration:**  
  Connects to a custom-built RESTful API developed with ASP.NET to handle:
  - User authentication & session management
  - Recipe queries & filtering
  - Ingredient matching logic
  - Meal planning data sync between platforms

- 📱 **Cross-Platform Support:**  
  Both mobile and web apps communicate with the same backend, ensuring seamless user experience across devices.

- 🧾 **Optional Features:**  
  - Ingredient recognition via camera (ML model or third-party API like Google ML Kit)
  - Smart grocery list generation (based on missing ingredients from selected meals)
  - Push notifications to remind users of planned meals

---


## 🌐 Web Application

### 🛠️ Tech Stack
- **Frontend:** HTML, CSS, JavaScript, ASP.NET MVC5
- **Backend:** C#, .NET Framework
- **Database:** MS SQL Server (Code-First Approach)
- **Frameworks/Libraries:** Entity Framework, Razor View Engine

### 🔑 Features
- User registration & login
- Ingredient input & smart recipe suggestion
- Personalized meal planner (calendar-based)
- View and filter recipes by ingredients, tags, and preferences
- Admin panel for recipe moderation
- Responsive design for desktop and tablet

### 📂 Main Pages
- `WelcomePage.cshtml`: Landing page for the app
- `SmartChef.cshtml`: Ingredient-based recipe search
- `MealPlanner.cshtml`: Weekly meal planning tool
- `RecipePage.cshtml`: Full recipe display with steps and ingredients

---

## 📱 Mobile Application

### 🛠️ Tech Stack
- **Framework:** Flutter
- **Language:** Dart
- **Architecture:** MVC / MVVM (depending on implementation)
- **Backend Communication:** REST API calls to the web service

### 🔑 Features
- Login/Register via shared account system
- Camera access to scan ingredients (optional)
- Display AI-generated or filtered recipes
- Save favorite recipes locally
- Sync planner with web version
- Push notifications for meal reminders

---

## 🔗 API & Database Integration

- Web and mobile apps share the same backend and SQL Server database.
- APIs are exposed using ASP.NET Web API or controller endpoints.
- Uses Entity Framework for Code First migration and schema management.

---

## 📸 Screenshots

### Web Interface

<p align="center">
  <img src="https://github.com/user-attachments/assets/d64d2800-a247-46c5-93ab-3f5116066d31" width="220"/>
</p>

### Mobile Interface

<p align="center">
  <img src="https://github.com/user-attachments/assets/ce61f96e-273d-4530-b73d-eaf222da351c" width="220"/>
 <img src="https://github.com/user-attachments/assets/aaa47a0f-9d4a-4601-a431-fe42aad9abd6" width="220"/>
 <img src="https://github.com/user-attachments/assets/339e6ee7-6eb0-436c-8a37-78cd5bedf11f" width="220"/>
 <img src="https://github.com/user-attachments/assets/ac333469-47fe-4250-9334-d20e39d3c70f" width="220"/>
</p>
---

## 🧪 How to Run the Project

### Web
```bash
# Clone the project
git clone https://github.com/yourusername/smartchef.git

# Open in Visual Studio
# Restore NuGet packages
# Update the connection string in Web.config

# Run the project
Ctrl + F5

```
### Mobile
```bash
# Clone the project
cd smartchef_mobile

# Get dependencies
flutter pub get

# Run on emulator or device
flutter run

```
## 🧩 Project Structure

```plaintext
SmartChef/
├── Web/
│   ├── Controllers/
│   ├── Models/
│   ├── Views/
│   ├── Scripts/
│   └── SmartChefDbContext.cs
├── Mobile/
│   ├── lib/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── widgets/
│   │   └── main.dart
├── Database/
│   └── Migrations/
│   └── smartchef.mdf

```

## 🧰 Requirements
- Visual Studio 2022+ (for web)
- SQL Server Express or higher
- Flutter SDK (3.x or later)
- Android Studio or emulator
- REST client (Postman, Thunder Client) for API testing

## 🧠 Future Improvements
- 🧠 Integration with AI recipe recommendation using GPT
- 🧺 Shopping list generator based on planner
- 🧭 Voice assistant integration (Google / Alexa)
- 🛒 API sync with grocery delivery platforms

## 🤝 Contributing
Want to help improve SmartChef?
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Submit a Pull Request ✅
