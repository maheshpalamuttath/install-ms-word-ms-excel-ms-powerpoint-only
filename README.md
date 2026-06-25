# ✅ Install ONLY Word, Excel, PowerPoint (Office 2019 via ODT)

---

## 🔹 STEP 1: Create folder

```text id="odtfolder"
C:\ODT
```

---

## 🔹 STEP 2: Download Office Deployment Tool

Download from Microsoft:

[Office Deployment Tool](https://www.microsoft.com/en-us/download/details.aspx?id=49117&utm_source=chatgpt.com)

Extract it to:

```text id="extractodt"
C:\ODT
```

(You should see `setup.exe`)

---

## 🔹 STEP 3: Create config file

Open Notepad → paste:

```xml id="configxml"
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

```text id="saveconfig"
C:\ODT\config.xml
```

---

## 🔹 STEP 4: Open Command Prompt (Admin)

* Press Windows key
* Type `cmd`
* Right-click → **Run as Administrator**

---

## 🔹 STEP 5: Go to ODT folder

```cmd id="cdodt"
cd C:\ODT
```

---

# 🔥 STEP 6: Choose ONE of these scenarios

---

## 🟢 SCENARIO A — Recommended (Online install)

👉 Use this if you have internet

```cmd id="scenarioA"
setup.exe /configure config.xml
```

✔ Downloads + installs in one step
✔ Simplest method
✔ Best for your setup

---

## 🟡 SCENARIO B — Offline / Pre-download method

👉 Use this if:

* slow internet OR
* you want backup installer files

```cmd id="scenarioB1"
setup.exe /download config.xml
setup.exe /configure config.xml
```

✔ First downloads Office files
✔ Then installs from local cache
✔ Useful for reuse or multiple PCs

---

# 📌 STEP 7: Finish installation

After completion, open Start Menu:

You will see:

* Microsoft Word
* Microsoft Excel
* Microsoft PowerPoint

---
---

# 🔹 STEP 8: Activate Office

Open Word → Sign in or enter product key.

---
