# Kindergarten Management Android App

This project presents an Android-based application designed to streamline the operational and managerial tasks of a kindergarten. Built with **Firebase** and developed by a **team**, the app simplifies managing students, staff, and parents through a user-friendly interface and core functionalities like **Create, Read, Update, and Delete (CRUD)** operations.

---

## About The App

The Kindergarten Management App was created to enhance data management and reduce paperwork in educational institutions for young children. It offers real-time synchronization, secure authentication, and intuitive navigation to ensure a seamless experience for administrators and staff.

---

## Objectives

- Design and develop an Android application for kindergarten management.
- Implement full CRUD operations for students and staff.
- Integrate **Firebase** for secure, real-time data handling.
- Use **Firebase Authentication** and **Cloud Firestore** to ensure data accessibility and protection.
- Create a responsive and intuitive user interface for easy interaction.

---

## CRUD Operations Overview

### Create
When users register via the **Sign-Up** button, inputs are validated and a new user is created using `createUserWithEmailAndPassword()` from Firebase Authentication. Upon success, extra details like name and phone number are stored in **Firestore**.

### Read
The `loadBabies()` function retrieves a list of registered babies for the user, displaying each baby in a card with their name, age, gender, and ID. It auto-refreshes on app launch or when changes occur.

### Update
In the profile section, the `onViewCreated()` method captures profile edits. After clicking "Save", the data is updated in **Firestore**, with confirmation or error messages shown based on the result.

### Delete
When users choose to delete their account, a confirmation dialog appears. If confirmed, the app deletes the user’s **Firestore** document and **Firebase Auth** account. Users are then signed out and redirected to the login screen.

---

## Developed by a Team

This project was built collaboratively by a dedicated team committed to improving the management of early education environments through modern technology.

---

## 💡 Technologies Used

- Android (Java)
- Google Firebase (Authentication + Firestore)
- Material Design UI Components
