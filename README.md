# Open Visual Studio Code From Finder On Mac


## Demo
Open your folder and file with VS Code from Finder with a subtle right click!

![Open VS Code from Finder](https://github.com/nmrenyi/open-vscode-from-finder-on-mac/raw/main/pics/demo.gif)

No more opening VS Code and selecting the lengthy path or dragging folders or files to VS Code any more!

## Motivation
It's quite a common need to open VS Code from Finder on Mac, especially for those developers who have been accustomed to opening VS Code from File Explorer in Windows with just a slight right click on the target folder or file.

However, VS Code on Mac does not offer this shortcut natively. So here is an **easy** and **subtle** way to implement this feature.

## Steps To Implement
1. Launch *Automator* on your Mac. 
2. Select *New Document* icon on the bottom of the window (highlighted with red box). ![step2-select-new-doc](https://github.com/nmrenyi/open-vscode-from-finder-on-mac/raw/main/pics/step2-new-doc.png)
3. Choose *Workflow* as the type for your document. ![step3-select-workflow](https://github.com/nmrenyi/open-vscode-from-finder-on-mac/raw/main/pics/step3-select-workflow.png)
4. Find the 4th category in the *Library* list on the left side of the window. Click on it and find *Open Finder Items*. Doubt click on this term or drag it to the pane on the right. ![step4-select-open-finder-item](https://github.com/nmrenyi/open-vscode-from-finder-on-mac/raw/main/pics/step4-select-open-finder-item.png)
5. Choose *Visual Studio Code.app* as the application of *Open with* drop down menu. ![step5-select-vscode](https://github.com/nmrenyi/open-vscode-from-finder-on-mac/raw/main/pics/step5-select-vscode.png)
6. Press `Command-S` to save the script to your favourite folder with your favourite script name. Done :)

Notes:
1. *Automator* is a powerful tool natively available in macOS, which aims to design and automate user customized workflow. To open *Automator*, you can find it from `Application` folder or simple search for it with *Spotlight*. See [Automator User Guide](https://support.apple.com/guide/automator/welcome/mac) from Apple for more information.
2. *Visual Studio Code.app* may not appear in the drop down menu of step 5 as expected. You may need to choose *other* and find it. Usually the *Visual Studio Code.app* is in `Application` folder. If not, you may refer to the installation part of [Visual Studio Code on macOS](https://code.visualstudio.com/docs/setup/mac#_installation) to move it here so that you can find it in `Application` folder.

## TODO
1. Now the implementation method only works for opening VS Code with the selected folder or file. It would be great if we can also open VS Code with the current folder in Finder. However, I have not found a way to do this yet. If you have any idea, creating an issue or pull request is more than welcome :) ![todo1](https://github.com/nmrenyi/open-vscode-from-finder-on-mac/raw/main/pics/todo1.png)

## Reference
1. The implementation method refers to the second answer of [this post](https://stackoverflow.com/questions/64040393/open-a-folder-in-vscode-through-finder-in-macos) on StackOverflow. . I organised these steps into a doc with a demo here for everyone who may need it.
