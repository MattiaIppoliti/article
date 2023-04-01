---
title: "Obsidian Vault Integration"
tags:
- setup
weight: -3
---

## Setup
Obsidian is the preferred way to use Quartz. You can either create a new Obsidian Vault or link one that your already have.

### New Vault
If you don't have an existing Vault, [download Obsidian](https://obsidian.md/) and create a new Vault in the `/content` folder that you created and cloned during the [setup](notes/setup.md) step.

### Linking an existing Vault
The easiest way to use an existing Vault is to copy all of your files (directory and hierarchies intact) into the `/content` folder.

## Settings
Great, now that you have your Obsidian linked to your Quartz, let's fix some settings so that they play well.

Open Settings > Files & Links and look for these two items:

1. Set the **New link format** to **Absolute Path in vault**. If you have a completely flat vault (no folders), this step isn't necessary.
2. Turn **on** the **Automatically update internal links** setting.


![[notes/images/obsidian-settings.png]]*Obsidian Settings*

## Templates
Inserting front matter everytime you want to create a new Note gets annoying really quickly. Luckily, Obsidian supports templates which makes inserting new content really easily.

> [!WARNING]
> 
> **If you decide to overwrite the `/content` folder completely, don't remove the `/content/templates` folder!**


> [!WARNING] Warning
> 
> **This is a generical warning!**

Head over to Options > Core Plugins and enable the Templates plugin. Then go to Options > Hotkeys and set a hotkey for 'Insert Template' (I recommend `[cmd]+T`). That way, when you create a new note, you can just press the hotkey for a new template and be ready to go!

> 👀 Step 4: [Preview Quartz Changes](notes/preview%20changes.md)

## Latex

Block math works with two dollar signs `$$...$$`

$$f(x) = \int_{-\infty}^\infty
    f\hat(\xi),e^{2 \pi i \xi x}
    \,d\xi$$
	
Inline math also works with single dollar signs `$...$`. For example, Euler's identity but inline: $e^{i\pi} = -1$

Aligned equations work quite well:

$$
\begin{aligned}
a &= b + c \\ &= e + f \\
\end{aligned}
$$

And matrices

$$
\begin{bmatrix}
1 & 2 & 3 \\
a & b & c
\end{bmatrix}
$$
