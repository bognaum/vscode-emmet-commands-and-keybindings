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

- remove element 
	- [Emmet docs demo](https://docs.emmet.io/actions/remove-tag/) 
	- [demo below](#delete-tag-demo)
- select element content or whole element or parent element (balance in/out)
	- [Emmet docs demo](https://docs.emmet.io/actions/match-pair/) 
	- [demo below](#balance-out-demo)
- iterate by edit points after the abbreviation is expanded 
	- [Emmet docs demo](https://docs.emmet.io/actions/go-to-edit-point/) 
	- [demo below](#items-and-edit-points-demo)
- select a tag name and attributes to edit 
	- [Emmet docs demo](https://docs.emmet.io/actions/select-item/) 
	- [demo below](#items-and-edit-points-demo)
- wrap some html-code with abbreviation 
	- [Emmet docs demo](https://docs.emmet.io/actions/wrap-with-abbreviation/#wrap-with-abbreviation) 
	- [demo below](#wrap-everything-together)
- wrap with abbreviation the every line individually 
	- [Emmet docs demo](https://docs.emmet.io/actions/wrap-with-abbreviation/#wrapping-individual-lines)
	- [demo below](#wrap-the-every-line-individually)
- rename element
	- [demo below](#rename-tag-demo)
- and some other


## In this extension:
- Added a keybinding system for the most used commands. You may see the keybindings if you open the above submenu.
- Creates a [submenu](#menu-of-all-emmet-commands) of the editor title menu with all existing in VS Code Emmet commands. 
- The titles of existing in VS Code command have changed to more understandable.
- If you will add your own keybindings - you will see your keybindings in the above submenu.

## Keybindings
|   |   |
| - | - |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>E</kbd>                                                 | Expand abbreviation.           |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>A</kbd>                                             | Balance out.                   |
| <kbd>Alt</kbd>+<kbd><</kbd> / <kbd>Alt</kbd>+<kbd>></kbd>                                 | Previous / next edit point.    |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd><</kbd> / <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>></kbd> | Previous / next item.          |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>D</kbd>                                                 | Delete tag.                    |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>R</kbd>                                                 | Rename tag.                    |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>W</kbd>                                                 | Wrap with abbreviation.        |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>M</kbd>                                                 | Merge lines.                   |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>=</kbd>                                                 | Evaluate math expression.      |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>Alt</kbd>+<kbd>/</kbd>                                  | Toggle comment (to HTML only). |

## Notes:
- Not all commands existing in the [Emmet documentation](https://docs.emmet.io/) have implemented in VS Code.
- Assigned keybindings does not correspond to the keybindings of [Emmet documentation](https://docs.emmet.io/).

## Balance out demo
|   |   |
| - | - |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>A</kbd> | Select the content of an element, then the element with tags, then the content of parent element, ect. |

![Balance out](IMG/emmet-balance-out-01.gif)

## Wrap with abbreviation demo

### Wrap everything together
|                                           |
| -                                         |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>W</kbd> |

![Wrap](IMG/emmet-wrap-04.gif)

### Wrap the every line individually
|                                           |
| -                                         |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>W</kbd> |

![Wrap](IMG/emmet-wrap-03.gif)

## Rename tag demo

|                                           |
| -                                         |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>R</kbd> |

![Rename](IMG/emmet-rename-01.gif)

## Delete tag demo

|                                           |
| -                                         |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>D</kbd> |

![Rename](IMG/emmet-delete-02.gif)
![Rename](IMG/emmet-delete-01.gif)

## Items and edit points demo
|   |   |
| - | - |
| <kbd>Alt</kbd>+<kbd><</kbd>                 | Previous edit point. |
| <kbd>Alt</kbd>+<kbd>></kbd>                 | Next edit point.     |

|   |   |
| - | - |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd><</kbd> | Previous item.       |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>></kbd> | Next item.           |

![Rename](IMG/emmet-items-edit-points-01.gif)

## Menu of all Emmet commands.

[![hr01]][hr01]

| Keybinding                                               | Title                                         | Command                                             |
| -------------------------------------------------------- | --------------------------------------------- | --------------------------------------------------- |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>E</kbd>                | Emmet: Expand Abbreviation                    | ```editor.emmet.action.expandAbbreviation```        |
|                                                          |                                               |                                                     |
|                                                          | Emmet: HTML - Go to - Match Tag               | ```editor.emmet.action.matchTag```                  |
| <kbd>Alt</kbd>+<kbd>&gt;</kbd>                           | Emmet: HTML - Go to - Next Edit Point         | ```editor.emmet.action.nextEditPoint```             |
| <kbd>Alt</kbd>+<kbd>&lt;</kbd>                           | Emmet: HTML - Go to - Prev Edit Point         | ```editor.emmet.action.prevEditPoint```             |
|                                                          |                                               |                                                     |
|                                                          | Emmet: HTML - Select - Balance In             | ```editor.emmet.action.balanceIn```                 |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>A</kbd>            | Emmet: HTML - Select - Balance Out            | ```editor.emmet.action.balanceOut```                |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>&gt;</kbd>           | Emmet: HTML - Select - Next Item              | ```editor.emmet.action.selectNextItem```            |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>&lt;</kbd>           | Emmet: HTML - Select - Previous Item          | ```editor.emmet.action.selectPrevItem```            |
|                                                          |                                               |                                                     |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>D</kbd>                | Emmet: HTML - Delete Tag                      | ```editor.emmet.action.removeTag```                 |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>R</kbd>                | Emmet: HTML - Rename Tag                      | ```editor.emmet.action.updateTag```                 |
|                                                          | Emmet: HTML - Split / Join Tag                | ```editor.emmet.action.splitJoinTag```              |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>Alt</kbd>+<kbd>/</kbd> | Emmet: HTML - Toggle Comment                  | ```editor.emmet.action.toggleComment```             |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>W</kbd>                | Emmet: HTML - Wrap With Abbreviation          | ```editor.emmet.action.wrapWithAbbreviation```      |
|                                                          |                                               |                                                     |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>=</kbd>                | Emmet: Evaluate Math Expression               | ```editor.emmet.action.evaluateMathExpression```    |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>M</kbd>                | Emmet: Merge Lines                            | ```editor.emmet.action.mergeLines```                |
|                                                          | Emmet: Reflect CSS Value                      | ```editor.emmet.action.reflectCSSValue```           |
|                                                          | Emmet: Update ImageSize                       | ```editor.emmet.action.updateImageSize```           |
|                                                          |                                               |                                                     |
|                                                          | Emmet: Number - Increment - By One            | ```editor.emmet.action.incrementNumberByOne```      |
|                                                          | Emmet: Number - Increment - By One Tenth      | ```editor.emmet.action.incrementNumberByOneTenth``` |
|                                                          | Emmet: Number - Increment - By Ten            | ```editor.emmet.action.incrementNumberByTen```      |
|                                                          |                                               |                                                     |
|                                                          | Emmet: Number - Decrement - By One            | ```editor.emmet.action.decrementNumberByOne```      |
|                                                          | Emmet: Number - Decrement - By One Tenth      | ```editor.emmet.action.decrementNumberByOneTenth``` |
|                                                          | Emmet: Number - Decrement - By Ten            | ```editor.emmet.action.decrementNumberByTen```      |
