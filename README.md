<div align="center">

<!-- Animated Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=200&section=header&text=Windows%2011%20Pro&fontSize=60&fontColor=ffffff&fontAlignY=38&desc=🔑%20Product%20Key%20Activation%20Guide&descAlignY=58&descSize=20&animation=fadeIn" width="100%"/>

<!-- Badges -->
<p>
  <img src="https://img.shields.io/badge/Platform-Windows%2011-0078D4?style=for-the-badge&logo=windows11&logoColor=white"/>
  <img src="https://img.shields.io/badge/Edition-Pro-7B2FBE?style=for-the-badge&logo=windows&logoColor=white"/>
  <img src="https://img.shields.io/badge/Method-CMD-black?style=for-the-badge&logo=windowsterminal&logoColor=white"/>
  <img src="https://img.shields.io/badge/Status-Working%20✓-00c853?style=for-the-badge"/>
</p>

<p>
  <img src="https://img.shields.io/github/stars/elfordanson/windows_11_pro_productkey_activation?style=social"/>
  &nbsp;
  <img src="https://img.shields.io/github/forks/elfordanson/windows_11_pro_productkey_activation?style=social"/>
</p>

</div>

---

<br/>

<!-- Introduction -->
<div align="center">
  <h2>✨ What does this guide do?</h2>
  <p>This guide walks you through <strong>upgrading and activating Windows 11 Pro</strong> entirely via Command Prompt — no third-party tools, no downloads.</p>
</div>

<br/>

---

## 📋 Table of Contents

> Click any section to jump directly to it.

| # | Section | Description |
|---|---------|-------------|
| 1 | [🚀 Getting Started](#-getting-started) | How to open CMD as Administrator |
| 2 | [🧹 Clear License Keys](#-step-1--clear-existing-license-keys) | Remove old keys before starting |
| 3 | [🔍 Check Your Edition](#-step-2--check-your-edition) | Verify upgrade eligibility |
| 4 | [⚙️ Install Pro Edition](#%EF%B8%8F-step-3--install-pro-edition) | Run the Pro upgrade installer |
| 5 | [✅ Activate Windows](#-step-4--activate-windows-11-pro) | Fully activate your license |

---

<br/>

## 🚀 Getting Started

> **You must run CMD as Administrator. Follow the steps below carefully.**

<br/>

**Step 1 —** Press the keyboard shortcut below to open the **Run** dialog:

<div align="center">
  <kbd>⊞ Win</kbd> + <kbd>R</kbd>
</div>

<br/>

**Step 2 —** Type `cmd.exe` in the box:

<div align="center">
  <img src="https://github.com/elfordanson/windows_11_pro_productkey_activation/assets/116512676/0483880c-43c7-4144-81d6-bc781906aca0" width="400" alt="Run Dialog"/>
  <br/>
  <sub><i>Run Dialog — Type cmd.exe here</i></sub>
</div>

<br/>

**Step 3 —** Press <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Enter</kbd> to launch as **Administrator**, then click **Yes** on the UAC prompt.

You should now see a window like this:

<div align="center">
  <img src="https://github.com/elfordanson/windows_11_pro_productkey_activation/assets/116512676/e322f8ce-f447-4179-9a6d-afc2d301ae94" width="500" alt="Admin CMD"/>
  <br/>
  <sub><i>Administrator: Command Prompt</i></sub>
</div>

<br/>

---

## 🧹 Step 1 — Clear Existing License Keys

> These commands will safely remove any previously installed product keys.

Run the following commands **one by one**, clicking **OK** after each popup:

```cmd
slmgr.vbs /upk
```
> 🗑️ Uninstalls the current product key.

```cmd
slmgr.vbs /cpky
```
> 🔒 Clears the product key from the registry.

```cmd
slmgr.vbs /ckms
```
> 🌐 Clears the KMS server name.

<br/>

> [!TIP]
> A small message box will appear after each command. Simply click **OK** to continue.

<br/>

---

## 🔍 Step 2 — Check Your Edition

> Before upgrading, verify that **Pro** is available as a target edition.

```cmd
DISM /online /Get-TargetEditions
```

<br/>

<div align="center">

| Result | What to do |
|--------|-----------|
| ✅ `Professional` appears in the list | You can proceed with the upgrade for **free**! |
| ❌ `Professional` does **not** appear | Your Windows version may not support this method. |

</div>

<br/>

---

## ⚙️ Step 3 — Install Pro Edition

> Copy and paste each command below into your Administrator CMD window and press Enter.

```cmd
sc config LicenseManager start= auto & net start LicenseManager
```

```cmd
sc config wuauserv start= auto & net start wuauserv
```

```cmd
changepk.exe /productkey VK7JG-NPHTM-C97JM-9MPGT-3V66T
```

```cmd
exit
```

<br/>

> [!NOTE]
> The installer will begin and show a **"% complete"** progress message.
> Wait until it reaches **100%**. It is completely normal to see an error at the end.

<br/>

> [!IMPORTANT]
> When the error appears → click **Exit**, then **restart your PC**.
> After reboot, Windows will run updates and install features automatically. Just wait for it to finish.

After your PC restarts, go to **Settings → System → About** and confirm that **Windows 11 Pro** is now installed. 🎉

<br/>

---

## ✅ Step 4 — Activate Windows 11 Pro

> The edition is installed but not yet activated. Run these commands to complete activation.

Open CMD as Administrator again:

<div align="center">
  <kbd>⊞ Win</kbd> + <kbd>R</kbd> → type <code>cmd.exe</code> → press <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Enter</kbd>
</div>

<br/>

Now run the following three commands **in order**:

```cmd
slmgr /ipk W269N-WFGWX-YVC9B-4J6C9-T83GX
```
> 🔑 Installs the KMS client product key.

```cmd
slmgr /skms kms8.msguides.com
```
> 🌐 Sets the KMS activation server.

```cmd
slmgr /ato
```
> ✅ Triggers online activation.

<br/>

<div align="center">
  <h3>🎊 Congratulations! Windows 11 Pro is now Activated!</h3>
  <p>Go to <strong>Settings → System → About</strong> to verify your activation status.</p>
</div>

<br/>

---

<br/>

<!-- Footer CTA -->
<div align="center">

### 💬 Did this guide help you?

If this guide saved you time, consider leaving a ⭐ — it helps others find this repo!

[![Star this repo](https://img.shields.io/badge/⭐%20Star%20this%20Repo-302b63?style=for-the-badge)](https://github.com/elfordanson/windows_11_pro_productkey_activation)
[![Follow on GitHub](https://img.shields.io/badge/Follow%20on%20GitHub-24243e?style=for-the-badge&logo=github&logoColor=white)](https://github.com/elfordanson)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=120&section=footer&animation=fadeIn" width="100%"/>

</div>
