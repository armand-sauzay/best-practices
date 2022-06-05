# Command Line 101

This tutorial aims at showing how to get started using the terminal (it might be a bit non intuitive in the beginning but you wont regret it)

__list of all commands ran in this tutorial__

- you can delete command_line_tutorial and re run the following in order:
```bash
#print working directory
pwd

#go to root folder
cd

#potentially run mkdir code if it does not exist

#list files in folder
ls

#go to folder code
cd code

# if command_line_tutorial already exists, you can ignore the next comand remove using rmdir command_line_tutorial

#create a folder named command_line_tutorial
mkdir command_line_tutorial

#go to folder command_line_tutorial
cd command_line_tutorial

#create a file called myfile.txt
touch myfile.txt

#write 'Hello World!' in the above created file
echo 'Hello World!' >> myfile.txt

#Add a line to the above created file
echo 'This is added to the file because of >>, otherwise > overwrites' >> myfile.txt

#copy myfile.txt into a file named myfilecopy.txt
cp myfile.txt myfilecopy.txt

#remove myfile.txt
rm myfile.txt

#remove myfilecopy.txt
rm myfilecopy.txt

#go to folder one step above
cd ..

#remove folder created for this tutorial
rmdir command_line_tutorial
```

Let's see where our terminal currently is:

```bash
pwd
```

Navigate to the folder where you usually put your code (I would recommend having a folder named ```code``` in your root folder)

```bash
cd path/to/your/folder/of/code
```
- for me for instance, I have got a code folder under /Users/myusername so I can do the following
    ```bash
    cd
    cd code
    ```
    Explanation:
    - ```cd```: brings me back to my root folder
    - ```cd code```: changes my working directory to code

- create a folder named command_line_tutorial
    ```bash
    mkdir command_line_tutorial
    ```

- go to folder command_line_tutorial
    ```bash
    cd command_line_tutorial
    ```

- create a file called myfile.txt
    ```bash
    touch myfile.txt
    ```
- write 'Hello World!' in the above created file
    ```bash
    echo 'Hello World!' >> myfile.txt
    ```

- Add a line to the above created file
    ```bash
    echo 'This is added to the file because of >>, otherwise > overwrites' >> myfile.txt
    ```

- copy myfile.txt into a file named myfilecopy.txt
    ```bash
    cp myfile.txt myfilecopy.txt
    ```

- remove myfile.txt
    ```bash
    rm myfile.txt
    ```

- remove myfilecopy.txt
    ```bash
    rm myfilecopy.txt
    ```

- go to folder one step above
    ```bash
    cd ..
    ```

- remove folder created for this tutorial
    ```bash
    rmdir command_line_tutorial
    ```


## Useful links
- https://www.codecademy.com/article/command-line-commands
