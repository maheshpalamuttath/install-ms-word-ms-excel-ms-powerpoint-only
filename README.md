# Install ONLY Word, Excel, PowerPoint (Office 2019) using ODT

---

## 🔹 STEP 1: Create folder

Create this folder:

```text
C:\ODT
```

---

## 🔹 STEP 2: Download Office Deployment Tool

Download from Microsoft:

[Office Deployment Tool](https://www.microsoft.com/en-us/download/details.aspx?id=49117&utm_source=chatgpt.com)

Run it and extract everything into:

```text
C:\ODT
```

You should see:

* setup.exe

---

## 🔹 STEP 3: Create configuration file

Open **Notepad** → paste this:

```xml id="office2019lite"
<Configuration>
  <Add OfficeClientEdition="32" Channel="PerpetualVL2019">
    <Product ID="ProPlus2019Volume">

      <Language ID="en-us" />

      <ExcludeApp ID="Access"/>
      <ExcludeApp ID="Outlook"/>
      <ExcludeApp ID="OneNote"/>
      <ExcludeApp ID="Publisher"/>
      <ExcludeApp ID="Teams"/>

    </Product>
  </Add>

  <Display Level="Full" AcceptEULA="TRUE"/>
</Configuration>
```

Save as:

```text
C:\ODT\config.xml
```

⚠ Make sure it is **config.xml (not .txt)**

---

## 🔹 STEP 4: Open Command Prompt (Admin)

* Press Windows key
* Type `cmd`
* Right click → Run as Administrator

---

## 🔹 STEP 5: Go to ODT folder

```cmd
cd C:\ODT
```

---

## 🔹 STEP 6: Install Office

Run:

```cmd
setup.exe /configure config.xml
```

---

## 🔹 STEP 7: Wait for installation

* Downloads + installs automatically
* Takes 10–30 minutes

---

## 🔹 STEP 8: Open Office apps

After install, you will see:

* Microsoft Word
* Microsoft Excel
* Microsoft PowerPoint

---
---

# 🔹 STEP 9: Activate Office

Open Word → Sign in or enter product key.

---
