## Description

Generic makefile intended for C and C++ under GNU.  
Now Supporting dinamic linking with headers!!

## Why?

So you don't have to make yours

## Usage

Just edit the variables and run it!

variables are:

**Directories:**

	BASE_DIR: Where the main and functions reside
	OUTPUT_DIR: Where the binary will be created
	LIB_DIR: Where the library will be created
	OBJ_DIR: Where all the objects will be created

**Filenames:** (without the extension)

	OUTPUT_NAME: the binary name
	MAIN_NAME: the main name
	FN_FILES_NAMES: the non main code names
	LIB_NAME: the library name that will be created
	HEADERS_LOCATION: where to search for the headers for dinamic linking (inside of BASE_DIR)
		What is dinamic linking? some magical thing that lets you get away 
		with #include "foo.h" when foo.h is in a subdirectory (func/foo.h)

**Compiler:**

	COMPILER: gcc/g++

**Extensions:**

	EXTENSIONS: the code extension (not the headers)

**Options:**

	EXECUTE_AFTER_COMPILATION:
			if enable the binary will be executed after compilation
	EXECUTION_DATA:
			if enabled data of the execution will be shown.
			It can be vervose or very vervose.
			If very vervose is selected a file will be created (not working)
	COMPILATION_FLAGS:
			The binary compilation flags without the "-"

## Implementation

	git clone git@github.com:riera90/generic-makefile.git
	cd greneric-makefile
	mv * <working directory>
	cd <working directory>
Configure the variables

	make
And enjoy the binaries!

## Licence

Licensed under the [BSD-3 licence](https://github.com/riera90/generic-makefile/blob/master/LICENSE.md)


## Whant to colaborate?

Read [CONTRIBUTING.md](https://github.com/riera90/generic-makefile/blob/master/CONTRIBUTING.md)!
