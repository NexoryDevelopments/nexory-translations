# Contributing

Everything can be done directly in your browser.

## How to Submit
* **Update a language:** Open `<app>/<LANG>.json`, click the **Edit** (pencil) icon, update missing strings from `<app>/EN.json`, and click **Commit changes...** → **Create pull request**.
* **Add a language:** Copy `<app>/EN.json`, go to `<app>/`, click **Add file** → **Create new file**, name it `<LANG>.json` in uppercase (e.g., `DE.json`), paste, translate, and open a **Pull Request**.

## Rules
* **Translate values only:** Keep JSON keys exact (`"save": "Spara"`, not `"spara": "Spara"`).
* **Keep variables intact:** Never translate `{username}`, `%s`, or `\n`.
* **Do not edit `EN.json`**.
* **Do not translate:** Nexory, Nexory Clipping.

## Translate with AI
You can use an AI (ChatGPT, Claude, Gemini) to translate, then review the result before submitting. Paste this prompt along with the JSON:
```
Translate the values in this JSON file into **[Target Language]** for a desktop/software application UI.
Use natural, standard software terminology for **[Target Language]** (avoid literal word-for-word translations).
Keep all JSON keys, formatting, `\n` line breaks, and variables like `{username}` or `%s` completely unchanged.
Do not translate brand/product names: "Nexory", "Nexory Clipping".
Return only valid JSON.
```
## Agreement
By opening a pull request, you confirm the work is yours (or properly reviewed) and license it under [LICENSE](LICENSE) for use in closed-source Nexory software.
