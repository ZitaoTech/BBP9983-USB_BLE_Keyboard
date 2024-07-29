# [Tutorial about customizing your own keymap](https://github.com/ZitaoTech/zmk-config_9983)  
If you have any questions about the keymap or you want your own keymap but don't know how to make it, please contact me.

## Interpretation to the different firmware:

`bbp9983_default.uf2`: default firmware.  
`P9983_sticky_shift.uf2`: default firmware feature + sticky shift  

A sticky shift stays pressed until another key is pressed, By using a sticky shift, you don't have to hold the shift key to write a capital.  
Why sticky shift?  
Because the keyboard has no integrated diodes, so there might be some ghost typing when you hold some keys together like shift + X.  
So sticky shift is very useful when you want to type some letters capitalized.  
How to check which keys can't be pressed together?  
![image](https://github.com/user-attachments/assets/255d3c13-0ec3-49cb-af76-eb1ff772eb89)
Go to this [file](https://github.com/ZitaoTech/zmk-config_9983/blob/main/config/boards/bbp9983/bbp9983.dts) For those keys that start with same numbers, by the default firmware they are shift, X and B, when you hold shift and press X or B, the keyboard just won't output anything.
