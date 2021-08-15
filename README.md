## My Emacs workflow

### Minimal pipeline

  - Install emacs on WSL via `=sudo apt-get install emacs=`
  - Launch emacs with `=emacs=` command
  - Open a file with F10 menu
  - Edit file using org mode (various operations)
  - Save file **C-x C-s**
  - Exit Emacs **C-x C-c**

<div class="INSTALL drawer">

  - Running in cmder bash (ubuntu) with F10 to access menu
  - Windows MSI (bad russian font)
  - VSCode extension (no agenda view)

</div>

### Improvements \[4/4\]

  - \[X\] F10 may need Fnlock to work on Lenovo - use Fn-Esc.
  - \[X\] Configure terminal to resolve [key binding
    conflicts](https://emacs.stackexchange.com/questions/68105/how-to-use-ctrl-c-on-wsl-key-binding-conflict)
    like Ctrl-C. See also `=org-disputed-keys=` in [Orgmode
    conflicts](https://orgmode.org/manual/Conflicts.html).
  - \[X\] Launch emacs with filename `=emacs -nw EMACS.org=`
  - \[X\] Use Shift for selection and CUA mode with more familiar key
    bindings.

## Next steps

### TODO Questions \[0/1\]

  - \[ \] What does bottom line with ==-UUU(DOS)\*\*–F1== mean?
  - \[ \] How to remove it?

### TODO How to \[0/1\]

  - \[ \] See agenda view with all todos from this file
  - \[ \] Move line across headers, beyond own section
  - \[ \] Close agenda buffer

### SOMEDAY Not critical \[0/8\]

  - \[ \] Recalulcate list stats
  - \[ \] What is the difference between scheduled and deadline?
  - \[ \] Export from orgmode to other formats (pandoc)
  - \[ \] Add timestamp with current time
  - \[ \] Change selection color to lightblue (I did, but it did not
    save)
  - \[ \] View calendar
  - \[ \] [Reload on file
    change](https://emacs.stackexchange.com/questions/169/how-do-i-reload-a-file-in-a-buffer?newreg=a3feb7dd0515464f962f420449b8f1a5)

### DONE Finshed tasks \[5/5\]

  - \[X\] \* Use sterisk to add difficulty level / priority for plain
    text
  - \[X\] Add more cycling todo tags `=#+SEQ_TODO:=`
  - \[X\] Archive tasks
  - \[X\] Create a link
  - \[X\] Make a selection and copy selection
  - \[X\] Sort this list based on completion is C-c ^

## Editing in orgmode

### \<TAB\> is all you need

  - TAB shows/hides headers (quite powerful\!)
  - Shift-TAB opens all headers

### Editing a hyperlink

Use ==\[\[url\]\[\]\]== syntax or C-c C-l TODO: hyperlinks inside
documents.

### Getting around headers

  - Alt + left rightor changes header level
  - Alt + up or down moves lines around
  - Shift - arrow:
      - changes list numbering style
      - cycles TODO-DONE in header
      - selects in CUA mode

### Use timestamps

SCHEDULED: \<2021-08-15 Sun\>

As
[guide](https://orgmode.org/guide/Creating-Timestamps.html#Creating-Timestamps)
suggests:

  - C-c . for timestamp
  - S-arrow for change

### Checkboxes

  - You must type \[0/0\] or \[0%\] for checkbox
  - Only X counts for completion, not \`x\` or \`+\`
  - C-c C-c toggles and recalculates
  - Check Rainer König video [OrgMode E01S05:
    Checklists](https://www.youtube.com/watch?v=gvgfmED8RD4&list=PLVtKhBrRV_ZkPnBtt_TD1Cs9PJlU0IIdE&index=5&t=444s)

Sample cjekbox list \[2/3\], \[66%\]:

  - \[X\] Item 1
  - \[X\] Item 2
  - \[ \] Item 3

### Agenda

  - \[ \] C-a

## Emacs configuration

### Where is the config?

  - \~/.emacs is a file
  - \~/.emacs.d is a directory

### Setting org-support-shift-select and CUA options

  - Selecting with Shift is already built-in part of Emacs, but not
    org-mode
  - Start with 'M-x customize' to find options
  - Set CUA is part of F10 menu

## Small reference

### Concepts:

  - "buffer" - a screen that represents a file or Emacs own

### Notation:

\- \* is always a header

  - properties box has :NAME: and :END:

## Videos

Essential:

  - [Carsten Dominik keynote
    (2008)](https://www.youtube.com/watch?v=oJTwQvgfgMM)
  - [Rainer König lesson
    series](https://www.youtube.com/playlist?list=PLVtKhBrRV_ZkPnBtt_TD1Cs9PJlU0IIdE)

Extension:

  - [Evil Mode: Or, How I Learned to Stop Worrying and Love
    Emacs](https://www.youtube.com/watch?v=JWD1Fpdd4Pc)

## Blogs and success stories

Why Orgmode:

  - <https://blog.aaronbieber.com/2016/09/24/an-agenda-for-life-with-org-mode.html>
