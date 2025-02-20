## Coding Standards

## Introduction

When developing with Power Apps, it is not possible to name controls with the same name in the application.  
In workflow development, multiple people will be involved in the development. Since it is not possible to name controls with the same name even if they are on different screens, naming rules are important.  
This document defines the naming rules for controls and variables in Power Apps.  

Although Power Automate is not developed by multiple developers, it is important to be aware of the importance of creating a program that is easy to read for future maintenance and operation.  
However, we will define naming rules in Power Automate as well, because we want to be conscious of creating programs that are easy to read.

## Glossary

| # | Terminology | Explanation |
|---|-------------|-----------------------------------------------------|
| 1 | PascalCase | A method in which the first letter of each word is capitalized (e.g. PascalCase) |
| 2 | CamelCase | A method in which the first letter is lower-cased for the first word only (e.g. camelCase) |
| 3 | SnakeCase | Use underscores (_) between words (e.g. upper_snake_case) |
| 4 | Upper SnakeCase | A method of entering and stating words with underscores (_) between words and using all uppercase letters (e.g. UPPER_SNAKE_CASE) |


## Power Apps Coding Conventions

As duplicate naming is not allowed for controls in Power Apps, developers must adhere to the minimum coding conventions for control names in the screen.  

### About control names

#### Screen Name

For screen names, “Screen ID_Screen Name” should be set.  
Example: USR001_Top screen, etc.

#### Control name in screen

The screen ID shall be given at the beginning of the control name (required).  
Example: USR001_DateTimePicker1

Controls are automatically named by Power Apps when created (e.g. Label1)  
Detailed naming conventions can be added, but since they do not bring out the productivity-enhancing benefits of low-code development, they should be kept to a minimum.

The description method should be a combination of “Pascal case” and “Snake case.  
Basically, “screen ID_control name” is used as the snake case, but the control name should be written in the Pascal case.  
Screen IDs should be written in all capital letters.

##### (Recommended content) The following naming configuration is also highly maintainable

> 1. capitalize the starting letter for each word  
>
> 2. controls etc. belonging to a screen should be separated by underscores and inherit the higher level naming as follows.  
> screen_id_gallery_name_control_name
> > 3. 
> 3. controls may be prefixed (e.g. “lbl” for labels)  
> In that case, the prefix should be in lower case, and the naming after that should be in Pascal case
> > 3. the control may be prefixed (e.g. “lbl” for a label) > in which case the prefix should be lower case and the rest of the name in the Pascal case  
> 4.
> In the case of a modal window, add “MW” to the end of the modal window container name in the form of ScreenID_modalwindow_nameMW.  
> > Example: USR001_conEditMW etc.

##### Example of control prefix (cited from MS site)

| Control Name                          |Prefix|
|---------------------------------------|------|
| Badge                                 | bdg  |
| Button                                | btn  |
| Camera control                        | cam  |
| Canvas                                | can  |
| Card                                  | crd  |
| Charts                                | chr  |
| CheckBox                              | chk  |
| Combo box                             | cmb  |
| Component                             | cmp  |
| Container                             | con  |
| Dates                                 | dte  |
| Drop down                             | drp  |
| Form                                  | frm  |
| Gallery                               | gal  |
| Group                                 | grp  |
| Header                                | hdr  |
| Html text                             | htm  |
| Icon                                  | ico  |
| Image                                 | img  |
| Info Button                           | info |
| Label                                 | lbl  |
| Link                                  | lnk  |
| List box                              | lst  |
| Progress Bar                          | pbar |
| Rating                                | rtg  |
| Rich text editor                      | rte  |
| Shapes (rectangle, circle, and so on) | shp  |
| Slider                                | sld  |
| Tab List                              | tbl  |
| Table                                 | tbl  |
| Text input                            | txt  |
| Timer                                 | tmr  |
| Toggle                                | tgl  |
| Video                                 | vid  |
| Toolbar                               | tlb  |
| Number input                          | num  |
| Radio                                 | rdo  |
| Spinner                               | spn  |
| Avatar                                | avt  |


#Credits : TTSJ-Workflow Requirements Document (by : Itazu-san) 
