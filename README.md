# Smart Meal Planner with Nutritional Analysis 🍱

A magical meal-planning adventure inspired by the whimsical world of Studio Ghibli! This JavaFX desktop application transforms dietary preferences into delightful 7-day meal plans with comprehensive nutritional analysis.

![Java](https://img.shields.io/badge/Java-17-orange)
![JavaFX](https://img.shields.io/badge/JavaFX-17.0.2-blue)
![Maven](https://img.shields.io/badge/Maven-3.6.0+-green)
![Gson](https://img.shields.io/badge/Gson-2.10.1-red)

## 🌟 Project Overview

Developed as part of MCA Semester II at Alliance University, this application demonstrates advanced Java concepts including JavaFX GUI development, Maven dependency management, Java Module System (JPMS), and JSON serialization. The application features a beautiful Ghibli-inspired design with beige backgrounds, vibrant green buttons, and warm brown text.

### ✨ Key Features

- **🎯 Personalized Preferences**: Choose from Vegetarian, Low-Carb, or Balanced diet types
- **📅 Smart Meal Planning**: Generate complete 7-day meal plans with 1-5 meals per day
- **📊 Nutritional Analysis**: Comprehensive breakdown of calories, carbs, protein, and fat percentages
- **💾 Data Persistence**: Automatic saving of preferences and meal plans in JSON format
- **🎨 Ghibli-Inspired UI**: Beautiful, themed interface inspired by Studio Ghibli's food aesthetics

## 🛠️ Technology Stack

- **Programming Language**: Java 17
- **UI Framework**: JavaFX 17.0.2
- **Build Tool**: Maven
- **JSON Processing**: Gson 2.10.1
- **IDE**: Eclipse IDE for Java Developers (2024-09)
- **Version Control**: Git & GitHub

## 📋 System Requirements

### Hardware Requirements
- **Processor**: Minimum 1 GHz (recommended: 2 GHz or higher)
- **RAM**: Minimum 2 GB (recommended: 4 GB or higher)
- **Storage**: At least 500 MB free disk space
- **Display**: Minimum resolution 1024x768

### Software Requirements
- **OS**: Windows 10/11, macOS, or Linux
- **JDK**: Java Development Kit 17 or higher
- **Build Tool**: Maven 3.6.0 or higher
- **IDE**: Eclipse IDE 2024-09 or compatible IDE with Maven support

## 🚀 Getting Started

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Bellamkonda-Nokesh/Smart-Meal-Planner-Project.git
   cd Smart-Meal-Planner-Project
   ```

2. **Install JDK 17**
   - Download from [Oracle](https://www.oracle.com/java/technologies/downloads/)
   - Set `JAVA_HOME` environment variable

3. **Setup Eclipse IDE**
   - Install Eclipse IDE for Java Developers (2024-09)
   - Configure to use JDK 17
   - Import project as Maven project

4. **Run the Application**
   - Right-click on the project
   - Run As → Java Application
   - Select `MainApp` as the main class

### Alternative Maven Run
```bash
mvn clean javafx:run
```

## 🏗️ Project Architecture

```
src/main/java/
├── com.mealplanner/
│   ├── MainApp.java                 # Application entry point
│   └── module-info.java             # Module configuration
├── com.mealplanner.data/
│   └── DataManager.java             # JSON file I/O operations
├── com.mealplanner.gui/
│   ├── PreferencesPane.java         # Preferences UI
│   ├── MealPlanPane.java           # Meal planning UI
│   └── NutritionPane.java          # Nutrition analysis UI
├── com.mealplanner.model/
│   ├── UserPreferences.java        # User preferences model
│   ├── Meal.java                   # Meal data model
│   └── MealPlan.java               # Weekly meal plan model
└── com.mealplanner.planner/
    ├── MealDatabase.java           # Default meals database
    └── MealPlanner.java            # Meal planning logic

src/main/resources/
└── styles.css                      # Ghibli-inspired styling
```

## 🎮 How to Use

### 1. Set Preferences
- Open the **Preferences** tab
- Select your diet type (Vegetarian, Low-Carb, or Balanced)
- Choose meals per day (1-5)
- Click "Save Preferences"

### 2. Generate Meal Plan
- Navigate to the **Meal Plan** tab
- Click "Generate Meal Plan"
- View your personalized 7-day meal schedule
- Plan is automatically saved as `mealplan.json`

### 3. Analyze Nutrition
- Go to the **Nutrition** tab
- Click "Analyze Nutrition"
- View comprehensive nutritional breakdown:
  - Total weekly calories
  - Carbohydrate percentage
  - Protein percentage
  - Fat percentage

## 🎨 UI Design

The application features a unique Ghibli-inspired aesthetic:
- **Background**: Warm beige (#F5E5C0)
- **Buttons**: Soft green (#A8D5BA)
- **Text**: Rich brown (#5C4033)
- **Layout**: Clean tabbed interface for easy navigation

## 🧪 Sample Data

The application includes a default meal database with options like:
- **Breakfast**: Oatmeal, Scrambled Eggs
- **Lunch**: Grilled Chicken Salad, Pasta with Marinara
- **Dinner**: Vegetable Stir Fry, Salmon with Quinoa

## 💡 Development Challenges & Solutions

### 1. Gson Serialization Issue
**Problem**: JPMS restricted Gson's access to private fields
**Solution**: Added public getters/setters and configured `module-info.java` with `opens` directive

### 2. Module System Access
**Problem**: JavaFX couldn't access main application class
**Solution**: Added proper `exports` declaration in module configuration

### 3. Git Integration
**Problem**: Repository conflicts during initial push
**Solution**: Used `git pull --rebase` to resolve conflicts and maintain clean history



## 📚 Learning Outcomes

This project provided hands-on experience with:
- JavaFX desktop application development
- Maven build system and dependency management
- Java Module System (JPMS) implementation
- JSON data serialization with Gson
- Git version control and collaborative development
- Software debugging and problem-solving

## Acknowledgments

- **Eclipse IDE** for providing an excellent development environment
- **Studio Ghibli** for inspiring our whimsical, food-centric design philosophy
- **Alliance University Faculty** for guidance and support throughout development

## 📖 References

- [JavaFX Documentation](https://openjfx.io/)
- [Gson Documentation](https://github.com/google/gson)
- [Maven Documentation](https://maven.apache.org/)
- [Java Module System Guide](https://openjdk.java.net/projects/jigsaw/)

## 📄 License

This project is developed for educational purposes as part of MCA coursework at Alliance University.

---

**🌟 Star this repository if our culinary magic inspires you! 🌟**

*Completed: April 23, 2025*
