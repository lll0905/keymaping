linux xorg 快捷键设计方案:
=========================

移动操作:
========
1. ctrl + hjkl  			为方向键
2. ctrl + cmd + hjkl  		为区域选定键
3. ctrl + i 				为光标移动到行首
4. ctrl + o 				为光标移动到行尾
3. ctrl + u 				为光标移动到页首
3. ctrl + p 				为光标移动到页末
3. ctrl + f 				光标向前移动一个单词
3. ctrl + r 				光标向后移动一个单词

删除操作:
========
3. ctrl + d 				删除一个字符
3. ctrl + w 				向前删除一个单词
3. ctrl + del				删除到行首
3. ctrl + cmd + d			删除一行

复制操作:
========
3. ctrl + cmd + c			复制一行
3. ctrl + c  				复制选定区域
3. super + c  				复制选定区域


粘贴操作:
========
3. ctrl + v					paste 		
3. super + v  				paste


符号操作:
========
3. ctrl + ;					输入: '-' 		
3. ctrl + '					输入: '_'
3. ctrl + (					输入: ''

窗口操作:
=========
3. super + w					关闭标签页
3. super + q					关闭程序
3. super + tab					切换程序窗口
3. super + tab					切换程序窗口








============ arrow
c-h   left
c-j   down
c-k   up
c-l   rightow

============ edit with area
c-h pressing cmd | super   
c-h   left
c-h   left
c-h   left
c-h   left
c-h   left


============================================ end customized keyboard
remove Lock = Caps_Lock
remove Control = Control_L
keysym Control_L = Caps_Lock
keysym Caps_Lock = Control_L
add Lock = Caps_Lock
add Control = Control_L
============================================ end customized keyboard

xcape -e 'Control_L=Escape'

!
  ! Clear the modifiers
  !
  clear    lock
  clear    shift
  clear    control
  clear    mod1
  clear    mod2
  clear    mod3
  clear    mod4
  clear    mod5
  
  ! Remapping
  keycode  37 = F17 NoSymbol F17
  keycode  64 = Alt_L NoSymbol Alt_L
  keycode  66 = Control_L NoSymbol Control_L
  keycode  90 = Multi_key NoSymbol Multi_key
  keycode  91 = Mode_switch NoSymbol Mode_switch
  keycode 105 = Meta_R NoSymbol Meta_R
  keycode 107 = Menu Sys_Req Menu Sys_Req
  keycode 108 = Control_R NoSymbol Control_R
  keycode 127 = Redo Undo Redo Undo
  keycode 134 = Alt_R NoSymbol Alt_R
  keycode 135 = Control_R NoSymbol Control_R
  keycode 164 = Undo Redo Undo
  keycode 166 = Super_L NoSymbol Super_L
  keycode 167 = Control_L NoSymbol Control_L
  
  !
  ! Set the modifiers
  !
  add shift   = Shift_L Shift_R
  add control = Control_L Control_R
  add mod1    = Alt_L Alt_R
  add mod2    = Num_Lock
  add mod3    = Super_L
  add mod4    = Meta_R
  add mod5    = Mode_switch





