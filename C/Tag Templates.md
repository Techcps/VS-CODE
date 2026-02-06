

<div align="center" style="padding: 5px;">
  <h1>VS Code set-up for C/C++</h1>
  
  <a href="https://youtu.be/tpkAAO-m1Gw">
    <img src="https://img.shields.io/badge/Watch_Here-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch Here">
  </a>
</div>


---

# C/C++ Setup Guide (MSYS2 + VS Code)

---

## 🔧 Install GCC Toolchain (MSYS2 UCRT64)

### 1️⃣ Open the Compiler Terminal

Open the **MSYS2 UCRT64** terminal (compiler environment).

> ⚠ Make sure you open **UCRT64**, not MSYS or MINGW64.

---

### 2️⃣ Install the Required Toolchain

Run the following command:

```
pacman -S --needed base-devel mingw-w64-ucrt-x86_64-toolchain
```

💡 To paste inside the MSYS2 terminal, press:

Shift + Insert

When prompted:

```
Proceed with installation? [Y/n]
```

Type:

```
Y
```

Then press **Enter**.

Wait until the installation completes.

---

## ✅ Verify Compiler Configuration

Run the following commands:

```
gcc --version
g++ --version
```

> If version numbers are displayed, the compiler is installed and configured successfully.

> If you see `command not found`, make sure the compiler path is added correctly to the system environment variables.

---

# 🧩 Set C Tag Template (VS Code Snippet)

### Step 1: Open User Snippets

- Open VS Code  
- Press **Ctrl + Shift + P**  
- Type **User Snippets**  
- Select **c.json**

---

### Step 2: Add the Following Snippet

```json
{
  "C Basic Template": {
    "prefix": "ctag",
    "body": [
      "#include <stdio.h>",
      "",
      "int main() {",
      "    printf(\"Hello World\\n\");",
      "    return 0;",
      "}"
    ],
    "description": "Basic C program template"
  }
}
```

Save the file.

---

## 🚀 How to Use the Snippet

1. Create any `.c` file  
2. Type:

```
ctag
```

3. Press **Enter**

The full C program template will be generated automatically.

---

# 🎯 Setup Complete

Your C compiler and VS Code basic template are now ready.

----

<div align="center" style="padding: 5px;">
  <h3>📺 Don't forget to Like, Share & Subscribe!</h3>

  <a href="https://www.youtube.com/@TechcpsOfficial">
    <img src="https://img.shields.io/badge/YouTube-TechCPS-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube Channel">
  </a>
</div>


---


<div align="center" style="padding: 5px;">
  <h3>📱 Join US</h3>

  <a href="https://t.me/Techcps">
    <img src="https://img.shields.io/badge/Telegram_Channel-0088cc?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram Channel">
  </a>
  &nbsp;
  <a href="https://whatsapp.com/channel/0029Va9nne147XeIFkXYv71A">
    <img src="https://img.shields.io/badge/WhatsApp_Channel-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp Channel">
  </a>
  &nbsp;
  <a href="https://www.linkedin.com/company/techcps/">
    <img src="https://img.shields.io/badge/LinkedIn-TechCPS-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  &nbsp;
  <a href="https://twitter.com/Techcps_/">
    <img src="https://img.shields.io/badge/TwitterX-TechCPS-000000?style=for-the-badge&logo=x&logoColor=white" alt="TwitterX">
  </a>
  &nbsp;
  <a href="https://instagram.com/techcps/">
    <img src="https://img.shields.io/badge/Instagram-TechCPS-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram">
  </a>
  &nbsp;
  <a href="https://facebook.com/techcps/">
    <img src="https://img.shields.io/badge/Facebook-TechCPS-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook">
  </a>

  <h3>Thanks for watching and stay connected 🙂</h3>
</div>


---
