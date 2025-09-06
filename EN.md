# HPE MSA 2050 Password Recovery and Reset Guide

If you forget the password of your **HPE MSA 2050** storage, there is no need to worry. You can follow the steps below to reset the password and regain administrative access.

---

## Password Reset Steps

1. **Plan for Downtime**  
   Before starting, ensure you perform this operation during low network activity. Schedule the expected **downtime** and inform relevant users or teams.

2. **Connect via Console Cable**  
   Use the **mini-USB console cable** (provided with the device) to connect to one of the storage controllers.  
   > This cable provides direct access to the device's CLI.

3. **Identify the Console Port**  
   Check the console port number in **Device Manager**.  
   - If the console port is not detected, download and install the **required driver** from [this link](#).

4. **Connect Using a Console Software**  
   Use software like **PuTTY** to connect to the device.  
   - Upon successful connection, you should see the device's **CLI prompt**.

5. **Execute Restore Defaults Command**  
   - Enter `restoredefaults` as the **Username**.  
   - Enter the device **serial number** (highlighted in the image) as the **Password**.

6. **Controller Restart and Login with Default Credentials**  
   - The controller will restart.  
   - After the device boots up, log in using the **default credentials**:  
     ```
     Username: manage
     Password: !manage
     ```

7. **Success!**  
   Your device is now ready for use with the default password.
