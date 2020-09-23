<div align="center">

## load file to listbox


</div>

### Description

2 simple code that save items to a file and the other that load items to the listbox from the file visit my homepage at http://www.cyberway.com.sg/~dyrws 4 more app
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Dua Yong Rew](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/dua-yong-rew.md)
**Level**          |Unknown
**User Rating**    |5.0 (15 globes from 3 users)
**Compatibility**  |VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[VB function enhancement](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/vb-function-enhancement__1-25.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/dua-yong-rew-load-file-to-listbox__1-3393/archive/master.zip)





### Source Code

```
*** The Save Function ***
  Open App.Path & "\" & "playlist.dyr" For Output As 1
    For x = 0 To List1.ListCount - 1
      List1.ListIndex = x
      Print #1, List1.Text
    Next
  Close 1
*** The Load Function ***
  Open App.Path & "\" & "playlist.dyr" For Input As 1
    Do Until EOF(1)
      Line Input #1, st
      List1.AddItem st
    Loop
  Close 1
```

