https://blog.codepen.io/2014/02/21/vim-key-bindings/
https://benmccormick.org/2014/07/02/learning-vim-in-2014-vim-as-language

# Modes
i: enter insertion mode
v: enter visual/selection mode
ESC: back to standard mode

# Cursor Motion 
h: left
j: down
k: up
l: right
%: next matching bracket
$: end of line
^: first non-whitespace char
[: prev section
]: next section
{: prev blankline section
}: next blankline section
": access numbered/lettered buffer

# Verbs
q: quit
w: write
!: ignore changes
.: repeat last text changing commands
<: unindent + motion
>: indent
B: move back one word
d: delete
c: change
C: Change to EOL
D: delete to EOL
E: move to EOW
f: find forward
F: find backward
G: goto line number prefixed, or end
H: goto home= first line on screen
i: insert before
I: insert at start of line
J: join current line and next line
L: goto last line on screen
M: goto middle line on screen
o: open line below and enter insert mode
O: open line above and enter insert mode
u: undo
p: paste before
P: paste after
S: substitute current line
y: yank=copy
Y: copy line
a: insert after current char
A: insert after EOL
/: search text
x: delete single character

# Nouns
b: word backward
w: word
iw: inner word = current word
p: paragraph
ip: current paragraph
t: tag
it: current tag

