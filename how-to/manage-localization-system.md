---
icon: language
---

# Manage Localization System

Localization settings can be found in: **Project Settings -> Meet and Talk -> Localization**

<figure><img src="../.gitbook/assets/MAT_Background.png" alt=""><figcaption></figcaption></figure>

### **Adding a New Language**

To add a new language, in the **Available Language List** click the + Icon\
This will add a new language to the list, then you need to select the language you want to add from the list\
At the very end, you need to click **Generate C# Enum**

{% hint style="info" %}
In Future Updates \[Generate C# Enum] button will be replace by automated version
{% endhint %}

### **Managing Localization in Code**

{% code title="Get Localization Settings" %}
```csharp
LocalizationManager.Instance;
```
{% endcode %}

{% code title="Get Actual Used Language (In-Game)" %}
```csharp
LocalizationManager.Instance.SelectedLang();
```
{% endcode %}

{% code title="Change Selected Language (In-Game)" %}
```csharp
LocalizationManager.Instance.selectedLang = SystemLanguage.Polish;
```
{% endcode %}

