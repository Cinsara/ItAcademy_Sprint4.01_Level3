# 🧪 Level 3 - Postman Testing

This exercise focuses on testing the previously developed Spring Boot projects (Maven and Gradle) using **Postman**.

---

## 🚀 Objective

Use Postman to create and configure environments for testing both the Maven and Gradle versions of the REST API developed in earlier exercises.

---

## 🌐 Environment Setup in Postman

You will need to create **two separate environments** in Postman:

### 1. Maven Project Environment

| Variable | Value               |
|----------|---------------------|
| `server` | `http://localhost`  |
| `port`   | `9000`              |

### 2. Gradle Project Environment

| Variable | Value               |
|----------|---------------------|
| `server` | `http://localhost`  |
| `port`   | `9001`              |

---

## 🔧 Using Variables in Postman

Once you've created both environments, you can write your request URLs in the following format using variables:
`{{server}}:{{port}}/HelloWorld`

or

`{{server}}:{{port}}/HelloWorld2/YourName`


This allows you to quickly switch between environments (Maven and Gradle) without manually updating the URLs.

---

## ✅ Example Requests in Postman

Make sure the corresponding Spring Boot application is running before testing.

### GET `HelloWorld` with Request Parameter

`{{server}}:{{port}}/HelloWorld?nom=YourName`

### GET `HelloWorld2` with Path Variable

`{{server}}:{{port}}/HelloWorld2/YourName`

---

## 📝 Tips

- Use the **"Environment Quick Look"** (`eye` icon in the top right of Postman) to confirm that your environment variables are correctly set.
- Use the **"Manage Environments"** button to switch between the Maven and Gradle configurations.
- You can create **collections** in Postman to organize and re-use requests for both environments.

---

## 📦 Summary

| Environment | Port | Description                         |
|-------------|------|-------------------------------------|
| Maven       | 9000 | Testing the Maven-based project     |
| Gradle      | 9001 | Testing the Gradle-based project    |

