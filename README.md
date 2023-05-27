# About

This Git repository is used to build and release customized version of [lencx/ChatGPT](https://github.com/lencx/ChatGPT).

Most critically following customizations are included at the moment:

- Store markdown files with chat names instead of IDs and support subfolders by having **|** in chat titles.
- Windows exe is digitally signed
- Windows MSI is digitally signed
- Windows MSI uses [user installation mode](https://github.com/tauri-apps/tauri/issues/2319#issuecomment-1182846485)

**NOTE!!!** I'm using version numbering 1.0.10x here to avoid conflicting with original binary version.
To avoid causing issues auto update feature is also totally disabled from this so enable **Watch -> Custom -> Releases** on this repository instead of.

## Usage tips

- Create _private_ GitHub repository and check `C:\Users\<username>\.chatgpt` folder to it. Then you have those .md files even after you remove chats.
  You probably also want use `.gitignore` file like this with it:

```
cache_model/**
ChatGPT.log
chat.model.cmd.json
chat.notes.json
download/**
```
