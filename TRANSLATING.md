# Help Translate VieTweaks

Thank you for your interest in making VieTweaks available to more people! Translating the app is straightforward.

## Where to find the text

All the text used in the application is stored in XML resource files. 
You can find the reference files in the `assets` folder of this repository:
- `assets/strings_en.xml` (Base English)
- `assets/strings_vi.xml` (Vietnamese Translation)

## How to Translate

1. **Make a copy** of the base English file `strings_en.xml`.
2. **Rename the file** according to your target language. For example, if you are translating to Spanish, you might name it `strings_es.xml`.
3. Open the file in any text editor.
4. The file consists of `<string>` tags. Each tag has a `name` attribute which is an identifier for the app, and the text inside the tags is what gets displayed on the screen.
   
   *Example:*
   ```xml
   <string name="nav_home">Home</string>
   ```
5. **Only translate the text inside the tags.** Do NOT change the `name="..."` attribute, as the app relies on it to find the text.
   
   *Translated Example:*
   ```xml
   <string name="nav_home">Inicio</string>
   ```
6. **Handling special characters**: 
   - If your translation includes an apostrophe (`'`), you must escape it with a backslash (`\'`).
   - If you see placeholders like `%1$s` or `%d`, keep them exactly as they are in your translation. They will be replaced by dynamic data (like numbers or text) when the app runs.

## Submitting your Translation

Once you have completed your `strings_[lang].xml` file:
1. You can submit it via a **Pull Request** to this repository.
2. Alternatively, you can open an **Issue** and attach your translated XML file.

Our development team will review it and include it in the next update. Thank you for your contribution!
