Vim-Autoclose
=============

Based on
http://www.vim.org/scripts/script.php?script_id=1849

There are very simple ways to insert a closing brace by setting up a few mappings. The problem with all these approaches is that they break undo, history or both. This script is my sixth attempt at correcting this problem and the first one that has worked in all scenarios. 

Using this script, typing ``(`` will result in (|), where | is the cursor position and the double backticks are just marking input. Typing a ``)`` will move the cursor outside the parens. This moving outside works even in nested scenarios. Typing ``if(my_array['key`` results in if(my_array['key|']) and ``)`` gets you if(my_array['key'])|. 

The paired characters are: [, (, {, ", ' 
