# 🔐 Credential Capture Educational Demo

### *(Cybersecurity Awareness Project — HTML, CSS, JS + GitHub API)*

This project is a **live demonstration** showing how easily attackers can capture your **email and password** through simple webpages.
It is built **ONLY for educational and awareness purposes** to help people understand how phishing websites steal credentials in the background.

---

## 🚀 Project Overview

The webpage created in this project accepts an email and password.
When the user clicks **Submit**, the entered details are automatically stored in my GitHub repository inside a file named:

```
users.txt
```

This mimics how a malicious website can capture user credentials without their knowledge.

For transparency and learning, the API calls are kept **visible in this demo**.
In real cyberattacks, this process happens silently in the background.

---

## 🛠️ Technologies Used

* **HTML**
* **CSS**
* **JavaScript**
* **GitHub REST API (Contents API)**
* **GitHub Pages for hosting**

---

## 🎯 Purpose of the Project

This project was built to:

* Demonstrate how phishing websites capture login information
* Show how API calls can secretly store credentials
* Educate users on the dangers of entering details on untrusted websites
* Raise awareness about online security and data theft
* Explain the importance of verifying websites before entering sensitive data

This project is **not** a hacking tool — it is an educational model to understand how attackers operate.

---

## 🔗 Live Demo (Use Fake Credentials)

👉 **Demo Website:**
[https://psivasai970.github.io/](https://psivasai970.github.io/)

---

## 📁 Check Stored Credentials (users.txt)

👉 **GitHub users.txt file:**
[https://github.com/Psivasai970/Psivasai970.github.io/blob/main/users.txt](https://github.com/Psivasai970/Psivasai970.github.io/blob/main/users.txt)

You can enter test credentials on the demo page and verify that they are stored immediately in real time.

---

## 📹 Video Explanation

Many users were confused about how to verify the stored data, so I created a video demonstrating:

* How the project works
* Where credentials are stored
* How API calls are made

👉 **LinkedIn Video Post:**
[https://www.linkedin.com/posts/p-siva-sai-10686417a_psivasai970githubiouserstxt-at-main-activity-7399787873933385728-4MqC](https://www.linkedin.com/posts/p-siva-sai-10686417a_psivasai970githubiouserstxt-at-main-activity-7399787873933385728-4MqC)

---

## ⚠️ Security Disclaimer

This project stores **plaintext credentials** (for demonstration only).
It is intentionally insecure to help people understand real-world cyber threats.

Do NOT:

* Enter your real email or password
* Use this code for malicious purposes
* Deploy this system for actual authentication

In real-world systems:

* API keys must be hidden
* Passwords must be hashed
* Front-end pages should never store credentials directly
* Sensitive operations must be performed in secure backend servers

---

## 🧩 How It Works (Technical Explanation)

1. The user submits an email and password in the form.
2. JavaScript captures the input.
3. A GitHub API request (`PUT /repos/:owner/:repo/contents/:path`) is sent with:

   * The new line: `email,password,timestamp`
   * Base64-encoded content
   * The latest `sha` of the existing file
4. GitHub stores or updates `users.txt`.
5. The file updates instantly, allowing users to verify it live.

**Note:**
In real phishing attacks, these API calls are hidden and the user never knows their credentials are being stolen.

---

## 🧪 Features

* Live credential capture
* Real-time store into GitHub repo
* Retry logic for SHA conflicts
* Visible API operations for learning
* Hosted on GitHub Pages
* Educational video included

---

## 📚 Future Enhancements

* Add hashing explanation
* Build a backend-secure version
* Create a cybersecurity awareness presentation
* Add logging visualization
* Create a safe training mode for students

---

## 🤝 Contribution

This project is for learning purposes.
If you want improvements, ideas, or a secure version using backend APIs, feel free to raise an issue or request.

---

## 📧 Contact

If you want the full project explanation or help with cybersecurity demos, reach out on LinkedIn:

🔗 [https://www.linkedin.com/in/p-siva-sai-10686417a/](https://www.linkedin.com/in/p-siva-sai-10686417a/)

---
