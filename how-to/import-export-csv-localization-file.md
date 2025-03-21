---
icon: language
---

# Import / Export CSV Localization File

<figure><img src="../.gitbook/assets/MAT_Pro.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
### This Featureis available only in the **Pro Version**

Import / ExThis is one of many features available exclusively in the **Pro** version. To learn more about all the exclusive functionalities of **Pro Version**, check out this comparison: [\[Version Difference\]](../getting-started/quickstart.md)
{% endhint %}

A separate .CSV _(Comma-separated values)_ file can be generated for each Dialogue containing all translatable data

{% hint style="warning" %}
### Remember!

That only saved data is converted to CSV file
{% endhint %}

### How to Generate a CSV File with Translations

{% tabs %}
{% tab title="Dialogue Editor" %}
* In the upper right corner of the editor find the button “Export”.&#x20;
* After clicking it, File Explorer will open, where you can choose the location where you want to save the CSV file&#x20;
* After selecting the location, save the file
{% endtab %}

{% tab title="Inspector" %}
* In the upper right corner of the editor find the button “Export”.&#x20;
* After clicking it, File Explorer will open, where you can choose the location where you want to save the CSV file&#x20;
* After selecting the location, save the file
{% endtab %}
{% endtabs %}

### How to Load a CSV File with Translations

{% tabs %}
{% tab title="Dialogue Editor" %}
* In the upper right corner of the editor find the “Import” button.&#x20;
* After clicking on it, the File Explorer will open, where you can select the place where the CSV file is saved.&#x20;
* After selecting the file, click “Open” and the data from the file will be loaded into Dialog
{% endtab %}

{% tab title="Inspector" %}
* In the upper right corner of the editor find the “Import” button.&#x20;
* After clicking on it, the File Explorer will open, where you can select the place where the CSV file is saved.&#x20;
* After selecting the file, click “Open” and the data from the file will be loaded into Dialog
{% endtab %}
{% endtabs %}

{% hint style="danger" %}
### Remember!

In a CSV file, text containing a quote is enclosed in quotes, and original quotes are replaced with double quotes.\
\
Example:\
`Name`` `<mark style="color:yellow;">`"`</mark>`Nickname`<mark style="color:yellow;">`"`</mark>` ``Surname`  **->**   <mark style="color:green;">`"`</mark>`Name`` `<mark style="color:yellow;">`""`</mark>`Nickname`<mark style="color:yellow;">`""`</mark>` ``Surname`<mark style="color:green;">`"`</mark>
{% endhint %}

### Example of Data Structure (Converted to Table)

<table><thead><tr><th width="372">GUID ID</th><th width="196">English</th><th>Polish</th></tr></thead><tbody><tr><td>1c13e8b4-c831-4a8c-9b1f-33b7a8ee6b90</td><td>Hello</td><td>Cześć</td></tr><tr><td>ba35f36e-65d7-488d-9dea-364b80238d26</td><td>Quote in CSV</td><td>Cudzysłów w CSV</td></tr><tr><td>fa98a1b3-7263-4049-b044-26792bff70cd</td><td>"A ""Quote"" Z"</td><td>"A ""Cudzysłów"" Z"</td></tr></tbody></table>

### Example of Data Structure (Raw Data)

```csv
GUID ID,ENGLISH,POLISH
1c13e8b4-c831-4a8c-9b1f-33b7a8ee6b90,Hello,Cześć
ba35f36e-65d7-488d-9dea-364b80238d26,Quote in CSV,Cudzysłów w CSV
fa98a1b3-7263-4049-b044-26792bff70cd,"A ""Quote"" Z","A ""Cudzysłów"" Z"
```
