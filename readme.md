# uipath-secret

1)use balareva activity in uipath to import image to powerpoint slide->install balareva.powerpoint.activities first
2)use omnipage ocr to decode captcha in uipath->install uipath.omnipage ocr activity first
3)use extract graph to get image from excel->install balareva.excel.activities
4)to extract a single row from a datatable read one sheet in a datatable 2)now use build datatable and create same columns in it now use for each row and and put condition.if  condition is met use add data row activity and usebuild datatable object and use row.itemarray.. after use write range activity and pass datatable object
5)to use drag and drop facility in uipath click on item you want to drag and select click type as down..now use hover activity to to place the drag item ..again use click activity to finally drop the item and select click type as up
6)to add picture from folder to word use word application scope first->install uipath.word activity first...now use replace text or picture and supply file name in scope...


to create a custom package you need to have a visual studio and nuget package explorer
1)go to visual studio and create a project->visual C# and select class library
2)right click on references and add twi references 1)system.activities 2)syste.componentmodel.composition
3)edit namespace and class name as per your choice
4)[category("input")]
5)pulic inargument<String> firstname{get;set;}
6)pulic inargument<String> secondname{get;set;}
7)pulic outargument<String> fullname{get;set;}
8)now extend class with code activity
9)override execute method of code activity class
10)var firstname=firstame.get(context)
11)var secondname=secondname.get(context)
12)var result=firstname+secondname;
13)fullname.set(context,result)
14)select release and uild solution
15)now go to open containing folder >bin>debug/release
16)now open nuget package explorer->create new package
17)right click and select add lib folder->>again right click and select add existing file and select the dll file
18)now click on edit and select edit meadata and save to any folder 
19)copy the nugetpackage inside package folder of uipath
20)now go to uipath and go to manage packages and under local search your package and install
21)activity will be visible as per namespace name in C# file
22)use activity in your workflow as per your requirement
