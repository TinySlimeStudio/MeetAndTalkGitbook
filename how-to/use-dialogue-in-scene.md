---
icon: message
---

# Use Dialogue in Scene

### Set Up Dialogue in Scene

To set up Dialogue for a scene, you need to go through a few steps:

{% stepper %}
{% step %}
### **Setup UI**

You need to prepare the Dialogue UI as described in this part of the documentation ...
{% endstep %}

{% step %}
### **Interaction Object**

To use the dialogue, you must have a prepared object in the scene that can trigger the dialogue. For the purposes of the demo and documentation, I will describe an example using TriggerArea.cs, but it could be a different script allowing the use of Unity Events, for example:

* InteractionScript.cs in Hellish Battle - **2.5D Retro FPS**
* DemoInteraction.cs or TriggerArea.cs in **Meet and Talk**
{% endstep %}

{% step %}
### **Start Dialogue**

{% hint style="info" %}
Selected option starts Dialogue from random Start Node
{% endhint %}

{% tabs %}
{% tab title="Base Dialogue Start (1 Line)" %}
{% code title="Quick Start Dialogue" fullWidth="false" %}
```csharp
DialogueManager.StartDialogue(DialogueContainer SO);
```
{% endcode %}
{% endtab %}

{% tab title="Base Dialogue Start (2 Line)" %}
{% code title="Setup first then Start Dialogue" %}
```csharp
DialogueManager.SetupDialogue(DialogueContainer SO);
DialogueManager.StartDialogue();
```
{% endcode %}
{% endtab %}
{% endtabs %}

Pro Version

{% tabs %}
{% tab title="Specific Dialogue Start (1 Line)" %}
{% code title="Quick Specific Start" overflow="wrap" %}
```csharp
DialogueManager.SetupDialogue(DialogueContainerSO DialogueSO, string StartID);
```
{% endcode %}

{% hint style="info" %}
Using this function in **Free Version** will Start Dialogue from random Start Node
{% endhint %}
{% endtab %}

{% tab title="Specific Dialogue Start (2 Line)" %}
{% code title="Setup first then Specific Start" %}
```csharp
DialogueManager.SetupDialogue(DialogueContainer SO);
DialogueManager.StartDialogue(string);
```
{% endcode %}

{% hint style="info" %}
Using this function in **Free Version** will Start Dialogue from random Start Node
{% endhint %}
{% endtab %}
{% endtabs %}
{% endstep %}
{% endstepper %}

### **Change Dialogue UI In-Game** <a href="#change-dialogue-ui" id="change-dialogue-ui"></a>

With a simple function you can change the UI used for dialogues, it can be called in UnityEvent or in Script

```csharp
DialogueManager.SetupUI(DialogueUIManager);
```

### Change Dialogue Language

```csharp
LocalizationManager.Instance.selectedLang = SystemLanguage.Polish;
```

