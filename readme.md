# uipath-secret

1)use balareva activity in uipath to import image to powerpoint slide->install balareva.powerpoint.activities first
2)use omnipage ocr to decode captcha in uipath->install uipath.omnipage ocr activity first
3)use extract graph to get image from excel->install balareva.excel.activities
4)to extract a single row from a datatable read one sheet in a datatable 2)now use build datatable and create same columns in it now use for each row and and put condition.if  condition is met use add data row activity and usebuild datatable object and use row.itemarray.. after use write range activity and pass datatable object
