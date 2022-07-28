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
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>E</kbd>                | Expand abbreviation.           |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>A</kbd>            | Balance out.                   |
| <kbd>Alt</kbd>+<kbd><</kbd>                              | Previous edit point.           |
| <kbd>Alt</kbd>+<kbd>></kbd>                              | Next edit point.               |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd><</kbd>              | Previous item.                 |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>></kbd>              | Next item.                     |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>D</kbd>                | Delete tag.                    |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>R</kbd>                | Rename tag.                    |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>W</kbd>                | Wrap with abbreviation.        |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>M</kbd>                | Merge lines.                   |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>=</kbd>                | Evaluate math expression.      |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>Alt</kbd>+<kbd>/</kbd> | Toggle comment (to HTML only). |

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
| &nbsp;                                      |                      |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd><</kbd> | Previous item.       |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>></kbd> | Next item.           |

![Rename](IMG/emmet-items-edit-points-01.gif)

## Menu of all Emmet commands.

[![hr01]][hr01]

| Keybinding                                               | Command / Title                                                                                                   |
| -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>E</kbd>                | ```editor.emmet.action.expandAbbreviation```        <br/> Emmet: Expand Abbreviation                    |
| &nbsp;                                                   |                                                                                                         |
|                                                          | ```editor.emmet.action.matchTag```                  <br/> Emmet: HTML - Go to - Match Tag               |
| <kbd>Alt</kbd>+<kbd>&gt;</kbd>                           | ```editor.emmet.action.nextEditPoint```             <br/> Emmet: HTML - Go to - Next Edit Point         |
| <kbd>Alt</kbd>+<kbd>&lt;</kbd>                           | ```editor.emmet.action.prevEditPoint```             <br/> Emmet: HTML - Go to - Prev Edit Point         |
| &nbsp;                                                   |                                                                                                         |
|                                                          | ```editor.emmet.action.balanceIn```                 <br/> Emmet: HTML - Select - Balance In             |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>A</kbd>            | ```editor.emmet.action.balanceOut```                <br/> Emmet: HTML - Select - Balance Out            |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>&gt;</kbd>           | ```editor.emmet.action.selectNextItem```            <br/> Emmet: HTML - Select - Next Item              |
| <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>&lt;</kbd>           | ```editor.emmet.action.selectPrevItem```            <br/> Emmet: HTML - Select - Previous Item          |
| &nbsp;                                                   |                                                                                                         |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>D</kbd>                | ```editor.emmet.action.removeTag```                 <br/> Emmet: HTML - Delete Tag                      |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>R</kbd>                | ```editor.emmet.action.updateTag```                 <br/> Emmet: HTML - Rename Tag                      |
|                                                          | ```editor.emmet.action.splitJoinTag```              <br/> Emmet: HTML - Split / Join Tag                |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>Alt</kbd>+<kbd>/</kbd> | ```editor.emmet.action.toggleComment```             <br/> Emmet: HTML - Toggle Comment                  |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>W</kbd>                | ```editor.emmet.action.wrapWithAbbreviation```      <br/> Emmet: HTML - Wrap With Abbreviation          |
| &nbsp;                                                   |                                                                                                         |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>=</kbd>                | ```editor.emmet.action.evaluateMathExpression```    <br/> Emmet: Evaluate Math Expression               |
| <kbd>Alt</kbd>+<kbd>E</kbd>, <kbd>M</kbd>                | ```editor.emmet.action.mergeLines```                <br/> Emmet: Merge Lines                            |
|                                                          | ```editor.emmet.action.reflectCSSValue```           <br/> Emmet: Reflect CSS Value                      |
|                                                          | ```editor.emmet.action.updateImageSize```           <br/> Emmet: Update ImageSize                       |
| &nbsp;                                                   |                                                                                                         |
|                                                          | ```editor.emmet.action.incrementNumberByOne```      <br/> Emmet: Number - Increment - By One            |
|                                                          | ```editor.emmet.action.incrementNumberByOneTenth``` <br/> Emmet: Number - Increment - By One Tenth      |
|                                                          | ```editor.emmet.action.incrementNumberByTen```      <br/> Emmet: Number - Increment - By Ten            |
| &nbsp;                                                   |                                                                                                         |
|                                                          | ```editor.emmet.action.decrementNumberByOne```      <br/> Emmet: Number - Decrement - By One            |
|                                                          | ```editor.emmet.action.decrementNumberByOneTenth``` <br/> Emmet: Number - Decrement - By One Tenth      |
|                                                          | ```editor.emmet.action.decrementNumberByTen```      <br/> Emmet: Number - Decrement - By Ten            |
