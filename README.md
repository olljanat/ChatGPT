# About

This Git repository is used to build and release customized version of [lencx/ChatGPT](https://github.com/lencx/ChatGPT).

Most critically following customizations are included at the moment:

- Store markdown files with chat names instead of IDs and support subfolders by having **|** in chat titles.
- Windows exe is digitally signed
- Windows MSI is digitally signed
- Windows MSI uses [user installation mode](https://github.com/tauri-apps/tauri/issues/2319#issuecomment-1182846485)

**NOTE!!!** I'm using version numbering 0.12.10x here to avoid conflicting with original binary version. However it also means that when 0.13.0 version will eventually get released application will start notify about updates and it is not sure if update will works. If you want avoid that you can set `auto_update` to `disable` in `C:\Users\<username>\.chatgpt\chat.conf.json` and enable **Watch -> Custom -> Releases** on this repository.

**Pro tip** Create _private_ GitHub repository and check `C:\Users\<username>\.chatgpt` folder to it. Then you have those .md files even after you remove chats.
