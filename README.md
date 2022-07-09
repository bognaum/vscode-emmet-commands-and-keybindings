[hr01]: https://bognaum.github.io/vscode-emmet-commands-and-keybindings/IMG/screenshot-01-01.png
[hr02]: https://bognaum.github.io/vscode-emmet-commands-and-keybindings/IMG/screenshot-02.png
[hr03]: https://bognaum.github.io/vscode-emmet-commands-and-keybindings/IMG/screenshot-03.png

# Emmet commands and keybindings
According to [Emmet documentation](https://docs.emmet.io/) Emmet has three base features:

1. abbreviation expanding
2. Emmet actions - the commands for advanced editing of HTML code
3. Emmet snippets 

We all know about the first feature, but I suggest you pay attention to Emmet actions.

## Emmet actions
Emmet actions may be very useful. For example:

- [remove element](https://docs.emmet.io/actions/remove-tag/)
- [select element content or whole element](https://docs.emmet.io/actions/match-pair/)
- [iterate by edit points after the abbreviation is expanded](https://docs.emmet.io/actions/go-to-edit-point/)
- [select a tag name and attributes to edit](https://docs.emmet.io/actions/select-item/)
- [wrap some html-code with abbreviation](https://docs.emmet.io/actions/wrap-with-abbreviation/#wrap-with-abbreviation)
- [wrap with abbreviation every line individually](https://docs.emmet.io/actions/wrap-with-abbreviation/#wrapping-individual-lines)
- rename element
- and some other

But you need some way to use Emmet actions. This extension will help you offered you a special keybindings and menu.

## In this extension:
- Added a keybinding system for the most used commands. You may see the keybindings if you open the above submenu.
- Creates a submenu of the editor title menu with all existing in VS Code Emmet commands. 
- The titles of existing in VS Code command have changed to more understandable.
- If you will add your own keybindings - you will see your keybindings in the above submenu.

## Keybindings
- ```Alt+E, E``` - Expand abbreviation.
- ```Ctrl+Shift+A``` Balance out.

- ```Alt+<``` / ```Alt+>``` - Previous / next edit point.
- ```Ctrl+Alt+<``` / ```Ctrl+Alt+>``` - Previous / next item.

- ```Alt+E, D``` - Delete tag.
- ```Alt+E, R``` - Rename tag.
- ```Alt+E, W``` - Wrap with abbreviation.
- ```Alt+E, M``` - Merge lines.
- ```Alt+E, =``` - Evaluate math expression.
- ```Alt+E, Alt+/``` - Toggle comment (to HTML only).

## Notes:
- Not all commands existing in the [Emmet documentation](https://docs.emmet.io/) have implemented in VS Code.
- Assigned keybindings does not correspond to the keybindings of [Emmet documentation](https://docs.emmet.io/).

## Demo
### Balance out
```Ctrl+Shift+A``` - Select the content of an element, then the element with tags, then the content of parent element, ect.

![Balance out](IMG/emmet-balance-out-01.gif)

### Wrap with abbreviation 
Creating a list from the some lines of text (```Alt+E, W```).

![Wrap](IMG/emmet-wrap-03.gif)

Wrapping a piece of code in an HTML element (```Alt+E, W```).

![Wrap](IMG/emmet-wrap-04.gif)

### Rename tag 

```Alt+E, R```

![Rename](IMG/emmet-rename-01.gif)

### Delete tag 

```Alt+E, D```

![Rename](IMG/emmet-delete-02.gif)
![Rename](IMG/emmet-delete-01.gif)

### Items and edit points 

- ```Alt+<``` / ```Alt+>``` - Previous / next edit point.
- ```Ctrl+Alt+<``` / ```Ctrl+Alt+>``` - Previous / next item.

![Rename](IMG/emmet-items-edit-points-01.gif)

## Menu of all Emmet commands.

[![hr01]][hr01]

<!-- [![hr02]][hr02] -->

<!-- [![hr03]][hr03] -->
