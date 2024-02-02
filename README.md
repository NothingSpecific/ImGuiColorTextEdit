# ImGuiColorTextEdit
Syntax highlighting text editor for ImGui

This [ImGuiColorTextEdit](https://github.com/BalazsJako/ImGuiColorTextEdit) fork was created for my own project, [Perplexed](https://github.com/NothingSpecific/Perplexed). It contains noteworthy changes from the original ImGuiColorTextEdit API, which may affect your use of it if you want to use it for your own project.

If you want an up-to-date fork to use for your own project, I recommend the [fork by santaclose](https://github.com/santaclose/ImGuiColorTextEdit) which seems to be well-maintained. While you're welcome to use this, the API may change without warning.

![Screenshot](https://github.com/BalazsJako/ImGuiColorTextEdit/wiki/ImGuiTextEdit.png "Screenshot")


# Noteworthy changes:

- Predefined language definitions return pointers to instantiated objects, not static references like they used to. This means they must subsequently be `delete`d to avoid memory leaks.

