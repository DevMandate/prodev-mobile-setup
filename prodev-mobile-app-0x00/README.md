# First Mobile App with Expo

## Objective
The purpose of this task was to create my first mobile application using the **Expo Router template**, understand the initial project structure, and run the app successfully on a physical device using Expo Go.

---

## Steps Followed

### 1. Navigate to Project Directory

cd prodev-mobile-setup
mkdir prodev-mobile-app-0x00
cd prodev-mobile-app-0x00

### 2. Initialize a New Expo Project
**npx create-expo-app@latest .**
This command scaffolded a new React Native project with Expo Router support.

### 3. Modify the Home Screen
Opened the file: **app/(tabs)/index.tsx** 
Located the default text: **<ThemedText type="title">Welcome!</ThemedText>**
Changed it to: **<ThemedText type="title">First App Created</ThemedText>**

### 4. Run and Test the App
Started the development server: **npx expo start**
- Android: Scanned the QR code using Expo Go app.
- iOS: Scanned the QR code using Camera app.
- The updated text First App Created displayed successfully.

### 5. Reset the Project
Ran the reset command: **npm run reset-project**


## Observations from reset-project
I was prompted with the following message:
*Do you want to move existing files to /app-example instead of deleting them? (Y/n):*

I chose Y, and the following happened:
- A new directory /app-example was created.
- The existing folders (/app, /components, /hooks, /constants, /scripts) were moved into /app-example.
- A fresh /app directory was created with default files:
   - app/index.tsx
   - app/_layout.tsx
- The reset ensured my project was in a clean state, while still keeping a copy of my previous work in /app-example for reference.

## File Structure Overview
Some important files and folders created by Expo:

prodev-mobile-app-0x00/ <br>
├── app/                   # Freshly scaffolded app folder <br>
│   ├── index.tsx          # New home screen <br>
│   └── _layout.tsx        # Default layout <br>
├── app-example/           # Backup of previous work <br>
│   └── app/(tabs)/index.tsx   # Modified screen ("First App Created") <br>
├── constants/Colors.tsx   # Default color theme <br>
├── package.json           # Project metadata and dependencies <br>
├── README.md              # Documentation for this task <br>