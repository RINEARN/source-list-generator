# SourceListGenerator.vcssl

A script for generating a list file of Java&reg; source files, useful when you compile them by "javac" command.

This script is written in the VCSSL. You can get the runtime environment from: [https://www.vcssl.org/en-us/](https://www.vcssl.org/en-us/)

## About a "List Files" and This Tool

When you compile multiple java source files by using "javac" command (whithout using build-tools or IDEs), you may describe pathes of all source files in a file (e.g. spurcelist.txt), and you can specify it as follows:

    javac @spurcelist.txt

where an example of the content of "spurcelist.txt" is:

    my/package/MyClass1.java
    my/package/MyClass2.java
    my/package/MyClass3.java
    ...

This script generates a list file like the above "spurcelist.txt", automatically.


## How to Use

### Step-1. Put the Script

At first, put the script "SourceListGenerator.vcssl" in your source code directory. 
Subdirectories will be traversed recursively, so put the script at the top hierarchy in the tree of source code directories.

### Step-2. Downlaod VCSSL Runtime and Extract

Then, download the runtime environment of the VCSSL (VCSSL Runtime) from: https://www.vcssl.org/en-us/ . Extract the downloaded ZIP file "vcssl_\*\_\*\_\*.zip" (where \*\_\*\_\* are version numbers) from right-click menu.

### Step-3. Execute the Script

Finally, launch the VCSSL Runtime and execute the script.

For Microsoft&reg; Windows&reg;, you can launch the VCSSL Runtime by double-clicking the batch file "VCSSL_\*\_\*\_\*.bat". For other environment, you can launch the VCSSL Runtime by the following command:

    cd <extracted_directory_of_VCSSL_runtime>
    java -jar VCSSL.jar

Then, a file choosing dialog will be displayed, so choose the script "SourceListGenerator.vcssl" which was put in your source code directory at the step-2. Then the script will be executed and "sourcelist.txt" will be output in the same directory.


## License

This script is released under [CC0](https://creativecommons.org/publicdomain/zero/1.0/deed).


---

## Credits

- Oracle and Java are registered trademarks of Oracle and/or its affiliates. 

- Microsoft Windows is either a registered trademarks or trademarks of Microsoft Corporation in the United States and/or other countries. 

- Other names may be either a registered trademarks or trademarks of their respective owners. 




