# Top Level Folders
## build
A REQUIRED folder used to store intermediate files which occurs between the 
source files and the final executable.  
It MUST NOT be checked into the Version Control System.
This folder is used for building the code.
Code may not be built in the same folder as the source files.

## src
A REQUIRED folder which is the primary location for source files created 
and edited for this component.
The folder may contain subfolders representing different splits in the code,
for example separate subfolders for different layers.
Private header files are also stored in this folder or subfolder.

## include
An OPTIONAL folder which contains public header files.
Public header files are those used by a higher level component which uses
the library being defined by this component.
If this component is generating an executable it will not need to have
a public header folder as there will be no public header files.
If this component is generating a library which can be used by another
library or executable then it will need to have a public include folder.

## tests
A REQUIRED folder which contains the tests for this component.
The tests may be further divided into subfolders representing different types
of tests, for example:
	unit, integration, functional, application, regression, stress, 
	end-to-end, acceptance, performance, smoke, stress, quality

## examples	
An OPTIONAL folder which contains examples showing how to use this component.

## external
An OPTIONAL folder containing third party components which are used by this 
component.  No files in this folder are edited.

## extras
An OPTIONAL folder containing extra or optional submodules for this component.

## data
An OPTIONAL folder containing non-source code files for this project.
For example, graphics files.

## tools
An OPTIONAL folder containging scripts, tool configurations, utilities.
For example, this folder may contain a subfolder called docker which contains
the dockerfile used by this project for CD/CI.

## docs
A REQUIRED folder containing project documentation.

## libs
An OPTIONAL folder for components used by this component.

