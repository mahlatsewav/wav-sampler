# 🎹 **Plugin Installation Guide**

A simple guide for installing your HISE‑built VST plugin.

---

## 📁 **What’s Inside**

Your downloaded folder should include:

* **wav-sampler.vst3** — The main VST3 plugin
* **wav-sampler.hr1** — Sample archive created by HISE
* **Presets/** *(optional)*
* **Samples/** *(only if using raw samples instead of HR files)*
* **README.md** *(this file)*

---

# 🪟 **Windows Installation (FL Studio, Ableton, Cubase, etc.)**

## **1. Install the VST3 plugin**

Move the `.vst3` file into the official VST3 folder:

```
C:\Program Files\Common Files\VST3
```

> FL Studio only scans the *official* VST3 folder. Do not place it anywhere else.

---

## **2. Install the HR1 sample file**

Place the `.hr1` file in:

```
Documents\wav-sampler\Samples
```

If the folder does not exist, create it manually.

Your final path should look like:

```
Documents
 └── wav-sampler
      └── Samples
          └── wav-sampler.hr1
```

---

## **3. Rescan Plugins in FL Studio**

1. Open **FL Studio**
2. Go to **Options → Manage Plugins**
3. Make sure this folder is listed under *Plugin search paths*:

```
C:\Program Files\Common Files\VST3
```

4. Click **Start scan**

Your plugin should now appear in:
**Add → More Plugins → Installed → VST3**

---

# 🔧 **Troubleshooting**

### **Plugin doesn’t appear in FL Studio**

* Ensure it is a **64‑bit VST3** plugin (HISE exports 64‑bit only).
* Verify the plugin is in:

  ```
  C:\Program Files\Common Files\VST3
  ```
* Rescan FL Studio plugins.

### **Plugin loads but samples are missing**

* Confirm your `.hr1` file is in:

```
Documents\wav-sampler\Samples
```

* Keep the filename exactly the same as the HISE export.
* Ensure the HR1 file was exported as **Monolith (HLAC)**.

### **Plugin crashes or loads empty**

* Try clearing the HISE sample cache:

```
Documents\HISE\SampleFolder\"Your Plugin Name"
```

* Rebuild your HR1 file from HISE.

---

