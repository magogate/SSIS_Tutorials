# SSIS_Tutorials from Pragmatic Works Cours - Introduction to SSIS
## Get the dataset
1.  You can download AdvendtureWorks databases backup files from https://github.com/Microsoft/sql-server-samples/releases/tag/adventureworks
2.  SSIS - I tried installing SSDT 2017 on Win 2019 server, however, that did not work - installation failed. Finally I downloaded SSDT 2015 and that worked. https://docs.microsoft.com/en-us/sql/ssdt/previous-releases-of-sql-server-data-tools-ssdt-and-ssdt-bi?view=sql-server-ver16 can be used to download prior releases of SSDT which you will find under section - "Privous SSDT releases"
3.  Or Try download Vistual Studio (2017 or anything else) Community Edition
4.  Download resources

## Module 00 - Getting Started 
  Just intro

## Module 01 - SSIS Overview
  Explanation of ETL and Cube etc
  
## Module 02A - Introduction to the Development Environment and the Control Flow
A. Solution File<br>
    1. SSIS Project<br>
      - SSIS Package1 **(dtsx)**<br>
      - SSIS Package2<br>
      - SSIS Package3<br>
    2. SSAS Project<br>
      -- SSAS Tabular Cube    <br>
    3. SSRS Project<br>
      -- SSAS Reports<br>
    4. SSIS Project 2<br>

- However, keep 1 sol - 1 proj - 1 tech
- To get the control windows -- Go to View Menu
- Go to Tools --? Options --> Project & Solutions --> Always show solutions (There are many things here)<br>
A. **Options**<br>
  1. Control Flow
  2. Data FLow
  3. Parameters
  4. Event Handlers
  5. Package Explorer
   


## Module 02B - Introduction to the Development Environment and the Control Flow
1.  Reusable - Create connection manager at project level instead of package level
    1. Right Click on Connection Manager Box - by default its a package level
    2. If you right click on "Connection Manager" from Solution Explorer - that way you create it at project level. This has ext as .conmgr and in bracket it says (project)
    3. or, you can change project conn to package conn or vice versa, by right clicking on connection itself at "Connection Manager Box"
3.  Naming Conventions - ProviderType_DatabaseType_databaseName e.g. OLEDB_SQL_PWInsurance 



## Module 02C - Introduction to the Development Environment and the Control Flow
1. Control flow is like Worklet or Mapplet
2. Tasks - inside control flow
3. Precedence Constraint - Sucess, Failure, Completion (And/Or)
  - Right click on link and select Success \ Failure \ Completion based on need
  - To get tool tip for sucecss -- Tool =--> Options --> Business Intelligence Designer ---> Integration Services Designer --> Show precedence constraint labels
5. Containers

To execute -- F5, Start or Right click on Package select Execute Package
To Stop  - Shift + F5, Stop or Click on URL

![image](https://user-images.githubusercontent.com/45523211/175368856-53b6175f-2e6b-49c1-8f3e-7f193ab649a4.png)

SSIS Toolbox (right hand corner icon)
![image](https://user-images.githubusercontent.com/45523211/175369014-012fe2ac-9ed7-455c-a603-92c6779aeba0.png)
