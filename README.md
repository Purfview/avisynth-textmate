<img width="971" height="534" alt="xxxCapture23" src="https://github.com/user-attachments/assets/aa262bdf-12d9-4801-beb1-771d0ec524d7" />


# AviSynth TextMate Highlighter

AviSynth syntax highlighting using a TextMate grammar.   
avisynth-textmate targets TextMate-compatible editors and provides the grammar metadata for [Visual Studio Code](https://code.visualstudio.com).   
It's also intended to be usable as an upstream grammar for GitHub Linguist.   
A prebuilt VS Code extension can be downloaded from the [Releases](https://github.com/Purfview/avisynth-textmate/releases) page.

The grammar is based on the [AviSynth syntax documentation](https://avisynthplus.readthedocs.io/en/master/avisynthdoc/syntax/syntax_sections.html).    
The AviSynth+ source code is at [AviSynth/AviSynthPlus](https://github.com/AviSynth/AviSynthPlus).


# Visual Studio Code guides

### Testing

1. Extract the repo ZIP.
2. In VS Code, open the extracted `avisynth-textmate-main` folder (the folder containing `package.json`).
3. Open Run > Start Debugging, or press F5.
4. In the new Extension Development Host window, open a `.avs` or `.avsi` file.
5. To inspect scopes, run **Developer: Inspect Editor Tokens and Scopes** from the Command Palette.

### Packaging

Install [Node.js](https://nodejs.org/) with npm, then run the following command from the repository root:

```cmd
npx.cmd @vscode/vsce package
```

This generates a `.vsix` extension package in the repository root.

### Installing the extension

In VS Code:
1. Open `View` > `Extensions` (`Ctrl+Shift+X`).
2. Open the `...` menu.
3. Select `Install from VSIX...`.
4. Select the generated `.vsix` file.

Alternatively, from the VS Code installation's `bin` directory, run the following command:

```cmd
code.cmd --install-extension "C:\path\to\avisynth-textmate-0.1.0.vsix" --force
```


