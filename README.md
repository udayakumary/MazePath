Repository:
Download solution from following path and extract the zip file. 
https://github.com/udayakumary/MazePath

Environment:
Developed this project using Visual Studio 2017 and .net framework 4.6.1. Technologies used for this project are c#, Web API, MVC, HTML, JQuery, CSS

What This Solution Contains?
Solution contains Web API (REST) service and client application (web page) to test web service. 
Service has one end point “SolveMaze” which accepts maze as input and returns solved maze and number of steps required to move from point A to point B.
Client application has two text box controls one to accept maze input and second to display solved maze. And it also displays number of steps required to move from “A” point to “B”.

How to Run This Application?
Open code in visual studio and Build it. Restore required packages through NuGet(If required) and run the application. 
Service will be self-hosted and client application page (Home page) will be displayed. Enter maze in “Input Maze” textbox and click on “Solve button”. Number of steps and output will be displayed.

To clear fields refresh page.

Logic Files: 
Rest Service:
Service/MapService.cs
Controller/MapController.cs
Test Page: Views/Home/Index.cshtml

Service Endpoint point:
http://localhost:8080/api/Map/SolveMaze

Assumptions:
1.Maze as two dimensional (All lines should be equal length) and surrounded by “#”
2.Contains only “#”, “.”, “A” and “B” characters
3.Only one start and end point
4.Contains at least one valid path otherwise same map will be return as out put
5.Always copy maze from notepad. 

Note:
All validations are not implemented. Client page is developed to test the service and logic, not focused on style sheets (As per phone conversation, only solution was requested)

