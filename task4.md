**Execution of the Task 4**


**Use the following instructions to get the gtkwave window**


ls - to check the contents of the folder


iverilog apeksha.v apeksha_tb.v - to simulate the verilog code and to check the errors


./a.out - to get the output and make vcd file to be ready open


![t41](https://github.com/1165111981/apeksha/assets/160841230/da2fa357-564f-442a-a5bd-907e306d71aa)


![t42](https://github.com/1165111981/apeksha/assets/160841230/615b2865-e240-41e0-8652-a8867f6e2f75)


**after running the command
gtkwave apeksha.vcd**


![t43](https://github.com/1165111981/apeksha/assets/160841230/ed3004fc-9670-4ffb-ae5e-529b9d0cad45)



**Before moving to the execution of the instructions let us understand few parts of a verilog code**

**-the code has been written in a systematic way and broken down into different parts**

1. Instruction Fetch Stage
   
   ![312794257-6009d228-beac-411e-a2ef-72ce8d6fad82](https://github.com/1165111981/apeksha/assets/160841230/3f222192-8d1c-4a17-b821-10fb1a4b7116)


2. Instruction Decode Stage

  ![312794650-0bf49697-4e9e-42dc-adcf-eed7df8e957c](https://github.com/1165111981/apeksha/assets/160841230/73f62a87-2087-4bb5-8977-63395d7b6dd3)


3. Contents of registers and registers used

 ![312795303-32ae2162-efe4-448a-afe2-7e850278e547](https://github.com/1165111981/apeksha/assets/160841230/516f93dc-89b5-47ab-8cab-f333c7b8e956)


4. Instructions Hardcoded

![312795521-23c86e3e-d2bd-4805-a8d3-2b1f6bde84c8](https://github.com/1165111981/apeksha/assets/160841230/c73eed81-cbb1-4c65-b1a3-60e30aef0d61)


**Lets move on to the execution Stage with Waveforms obtained for running the gtkwave apeksha.vcd**


1. When instantiated module is selected we get all the registers and wires as shown in the below figure
![t43](https://github.com/1165111981/apeksha/assets/160841230/c65fe436-c63e-4766-9b0a-4ec76fde3d40)



2. Upon adding few signals the waves can be see as shown in the below figure
![t45](https://github.com/1165111981/apeksha/assets/160841230/b824a1ac-1ac6-4e4f-8a6f-69472807bd1f)

**Output showing the ADD Operation**

![WhatsApp Image 2024-03-20 at 17 11 29_e7c2426c](https://github.com/1165111981/apeksha/assets/160841230/3991eb98-f345-488d-8e96-d298ec20fd3b)


**Output showing the SUB Operation**

![WhatsApp Image 2024-03-20 at 17 21 55_2cd8c05e](https://github.com/1165111981/apeksha/assets/160841230/7c2f45f6-ae63-4c8a-b5ca-6b85053ab33c)


**Output showing the AND Operation**

![WhatsApp Image 2024-03-14 at 14 51 11_9e3af44e](https://github.com/Abdulbitm/Abdul/assets/160620896/c4f77171-0166-4815-8d50-7820613c9b3a)


**Output showing the OR Operation**
![WhatsApp Image 2024-03-14 at 14 51 11_64d882fe](https://github.com/Abdulbitm/Abdul/assets/160620896/45ae0f92-78ab-469a-bacd-5cdb2f7c5578)

![WhatsApp Image 2024-03-14 at 14 51 11_c263287b](https://github.com/Abdulbitm/Abdul/assets/160620896/4d337702-67ac-4800-b7b6-b4bf4a7029f8)

**Output showing the XOR Operation**

![WhatsApp Image 2024-03-14 at 14 51 11_64d882fe](https://github.com/Abdulbitm/Abdul/assets/160620896/5584f6ad-a942-460b-a2d1-c44a1a68ca8e)

