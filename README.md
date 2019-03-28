
# General


**`Esc`**/**`Ctrl+c`** : 📣command mode

**`:q!`** : 🚪quit without saving

**`:wq`**/**`:x`** : ✅🚪save and quit

**`u`** : ↩️undo

**`Ctrl + r`** : ↪️redo

**`:set number`** : 🔢

---

# Insert

**`i`** : ⤵️insert before cursor
- **`I`** : insert at the beginning of line
- **`a`** : insert after cursor
- **`o`** : insert new line
- **`:r file`** : insert external file at the location of the cursor
- **`:#r file`** : insert external file at line number #

---


# Movement

## character

**`h`** : ⬅️Left

**`l`** : ➡️Right



## line

**`j`** : ⬇️Down

**`k`** : ⬆️Up

**`:#`** : jump to line number #
- or **`#G`** 

**`0`** : ⬅️jump to beginning of the line

**`$`** : ➡️jump to the end of the line



## word

**`w`** : ➡️next word (beginning)

**`e`** : ➡️next word (end)

**`b`** : ⬅️previous word (beginning)


## sentence

**`)`** : ➡️jump to the beginning of the next sentence 

**`(`** : ⬅️jump to the beginning of the previous word 


## paragraph

**`}`** : ➡️jump to the beginning of the next paragraph 

**`{`** : ⬅️jump to the beginning of the previous paragraph 


## page/screen

**`G`** : ⏭move screen to the end of the text

**`gg`** : ⏮move screen to the beginning of the text


**`Ctrl+f`** : ➡️next page

**`Ctrl+b`** : ⬅️previous page



---

# Search Pattern


**`/`** : ➡️search pattern (forward)
    
**`?`** : ⬅️search pattern (backward)

**`n`** : ➡️ / ⬅️find next (same direction)

**`N`** : ➡️ / ⬅️find next (opposite direction)


**`*`** : ➡️search current word (forward)
    
**`#`** : ⬅️search current word (backward)

---

# Editing 

## cut/copy/paste

**`d`** : ❌✂️delete/cut selection

use with motions: 
- **`de`** : delete rest of the word
- **`d)`** : delete rest of the sentence
- **`dd`** : delete a line
- **`d/?`** : delete until ? 



**`y`** : 📑copy

use with motions: 
- **`ye`** : copy rest of the word
- **`y)`** : copy rest of the sentence
- **`yy`** : copy line


**`x`** : ❌✂️cut character/selection

**`p`** : 📋paste (after the cursor)




## selection

**`v`** : 🔖select mode
- **`V`** : select line
- **`Ctrl+v`** : select block

## replace


**`r`** : ❌⤵️replace character
- **`s`** : delete character and insert
    
**`c`** : ❌⤵️replace entire line or selection

use with motions: 
- **`ce`** : replace rest of the word
- **`c)`** : replace rest of the sentence
- **`cc`** : replace a line
- **`c/?`** : delete until ? and replace with

**`:%s/old/new/gc`** : 👴⤵️👦replace old pattern with new (global/confirm)


---

# Jumps, Marks, & Registers

## Jump History

**`Ctrl + i`** : ⏩ move curser forward in history

**`Ctrl + o`** : ⏪ move curser backward in history

**`:jumps`** : 📜see list of jumps 
    
    


## Marks

**`ma`** : ◎ mark current position as a

**`'a`** : 🎯jump to mark a

**`'.`** : ⏪jump to last edit
    
**`:marks`** : 📜see list of marks 


## register

**`"ay`** : 📑copy to register a
    
**`"ap`** : 📋paste from register a
    
**`:reg`** : 📜see list of registers 


---


# Multiple Files, Buffers, & Tabs

## split view

**`:sp`** : 🏙🏙 split view (open new window/ same buffer)
- or **`Ctrl+ws`** 
- **`:vsp`** : split vertically

**`Ctrl + ww`** : 🏙🔄🏙 switch between windows

**`Ctrl + wc`** : 🏙close window

## Buffers

**`:e file`** : 🏙🌆 edit file in new buffer
- **`:e!`** : reload file from disc

**`Ctrl+g`** : ℹ️show file name and cursor location

**`:ls`** : 📜see list of all buffers 

**`:bn`** : 🏙➡️🌆 move to next buffer

**`:bp`** : 🏙⬅️🌆 move to previous buffer

- **`:b file`** : move to a specific buffer "file"
- **`:b #`** : move to buffer number #

## tabs

**`:tabnew`** : 🗂open new tab
- **`:tabnew file`** : open file in new tab

**`:tabn`** : ▶️🗂next tab

**`:tabp`** : 🗂◀️previous tab


