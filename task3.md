**By Referring to C-based Lab videos and RISC-V-based lab videos**

**Snapshots of the compiled C code and RISC-V**

**Step 1: check whether the leafpad is installed in ur machine by using the commands
leafpad sum1ton.c& (sum1ton.c is the file name)
If the leafpad editor is opened without any errors then type the C code.**
****If the leafpad is not installed in ur machine then install by using the following command**

**sudo snap install leafpad****
![Screenshot from 2024-02-27 10-23-29](https://github.com/1165111981/apeksha/assets/160841230/6f0333f3-6fea-43ac-8f24-e80e0a7ef2cc)


****Step 2: Writing the C code in the leafpad editor** using the following command

**leafpad sum1ton.c&**
![Screenshot from 2024-02-27 10-23-37](https://github.com/1165111981/apeksha/assets/160841230/477cc939-8131-42fa-80d0-f7364a66a126)


**Step 3: After writing the C code save the editor by Ctrl+s**

**Step 4: Check for the errors by using the following command(compilation step)**

**gcc sum1ton.c**
![Screenshot from 2024-02-27 10-24-11](https://github.com/1165111981/apeksha/assets/160841230/5fa334b5-f016-4a17-ae07-c854ea0a2ff6)


**Step 5: Check the output by using the command**

**./a.out**
![Screenshot from 2024-02-27 10-24-11](https://github.com/1165111981/apeksha/assets/160841230/7c25e189-8b79-4ed4-ad33-f80a5ec4a561)


**The results will be displayed as** 

**Sum of numbers from 1 to 350 is 61425**


********************************************************RISCV Compilation and Execution*****************************************************

**Step 1: View the C Code in the editor window using the following command**

**cat sum1ton.c**
![Screenshot from 2024-02-27 10-24-30](https://github.com/1165111981/apeksha/assets/160841230/c552b523-4e49-4bf8-ac31-8db446f04235)


**Step 2: Compile the code in riscv using the following command**

**riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c**


**Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.**

**use the command**

**ls -ltr sum1ton.c**

![Screenshot from 2024-02-27 10-34-54](https://github.com/1165111981/apeksha/assets/160841230/0125e636-3adc-4d56-8107-cc4e3f890ab0)





**Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution**

![Screenshot from 2024-02-27 10-34-54 (1)](https://github.com/1165111981/apeksha/assets/160841230/73850701-f79f-4a16-a548-ec569e025208)



**Step 4:**

**riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c**


![Screenshot from 2024-02-27 10-36-18](https://github.com/1165111981/apeksha/assets/160841230/a4a1fa39-527c-4a1d-a930-ffea92fda4a3)


![Screenshot from 2024-02-27 10-36-23](https://github.com/1165111981/apeksha/assets/160841230/111252ec-6b54-48e2-8ab4-ccefc315997c)





