<div align="center">

## Changing Object Fonts In Code @ RunTime


</div>

### Description

This little tutorial shows how to change the font on controls at runtime. Easy to do in the IDE, but, to do it in code at runtime in .NET (compared to VB6) it is a bit different!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Pooh\!](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/pooh.md)
**Level**          |Beginner
**User Rating**    |4.9 (49 globes from 10 users)
**Compatibility**  |VB\.NET
**Category**       |[Controls/ Forms/ Dialogs/ Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/controls-forms-dialogs-menus__10-3.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/pooh-changing-object-fonts-in-code-runtime__10-618/archive/master.zip)





### Source Code

<br><br>The reason for this tutorial:<br><br>Feeling like a newbie again after 5 years with VB, .NET poses some obsticals that I certainly was not prepared for.<br>Changing a font size was quick and easy in VB6, but in the .NET world, it proved itself to be a tedious task. My example is shown below:<br><br>
I have a solution with a blank form, and at runtime, all controls are dynamically built from a text file and placed in the window.<br><br>
The problem is that with .NET, all controls like this default to the form's font settings - And MS made the Font property of labels, etc. READ-ONLY.?<br><br>
In order to accomplish this, you need to create a new font object with your values, and assign it to your (Control).Font property.<br><br>
This will allow you to change the Font Family, the size in points, and the Bold / Italic etc. properties as well.<br>
<br>
<u>As an example, we are defining label "Label1" the Font Family "Arial", 8.25 Points in size, and BOLD.</u><br>
<b>Label1.Font = New Font("Arial", 8.25, FontStyle.Bold, GraphicsUnit.Point, 0, False)</b><br><br>
<br><u>You could also express it as:</u><br>
<b>Dim MyFont as New Font("Arial", 8.25, FontStyle.Bold, GraphicsUnit.Point, 0, False)
<br><br>
Label1.Font = MyFont<br><br>
Label2.Font = MyFont</b><br><br>
I hope this helps someone, as I was scratchin' hair out of my head over this. I
knew it could be done.<br><br> Funny thing is, it actually was pretty simple! <i>Heh</i>.<br><br>
John.

