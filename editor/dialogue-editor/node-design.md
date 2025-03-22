---
icon: message
---

# Node Design

<figure><img src="../../.gitbook/assets/Zrzut ekranu (82).png" alt=""><figcaption></figcaption></figure>

{% stepper %}
{% step %}
### Node Title & Description

A purely visual element that contains its name and a short description. It does not affect the dialogue logic but can be used for better organization and readability of the project.
{% endstep %}

{% step %}
### Node Button

The button next to the title allows adding new elements, such as **Choice** options, **Events**, and other functionalities that influence the dialogue flow.
{% endstep %}

{% step %}
### Node Input

An entry point of a node that can be connected to multiple other nodes.
{% endstep %}

{% step %}
### Node Output

An exit point of a node that determines which node will be executed next. A standard **Output Port** can only be connected to one node, except for the [**Random Output**](../functional-nodes/random-output.md), which allows randomly selecting one of multiple possible paths.
{% endstep %}

{% step %}
### Node Choice Outputs

Fields available in **Choice** nodes that enable the dynamic addition and removal of options. Each option can lead to a different node, allowing for the creation of multi-branching and interactive dialogues.
{% endstep %}

{% step %}
### Node Content

Special fields in nodes that store values, objects, variables, events, and other logical elements. These can be used to store information.
{% endstep %}
{% endstepper %}

