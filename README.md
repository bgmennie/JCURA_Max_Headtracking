**JCURA_Max_Headtracking**

Use this patch with the GyrOSC app for iOS to visualize head rotations and send OSC via UDP. 
This was used in a research paper to send values to Unity for in-game head tracking:
https://www.researchgate.net/publication/370864719_Creating_a_Low-Cost_Reproducible_Virtual_Mixing_Environment


Instructions:
1. Install the GyrOSC app for iOS from the app store on the headtracking phone
2. In GyrOSC, select the icon at the bottom left, and enter the IP address for the target computer running Max and an unused port (default for the patch is 8500)
3. In GyrOSC, select the icon at the middle left and ensure that the Gyroscope switch is enabled, and the Frequency is set to 120
4. Mount the headtracking phone to the top of a pair of headphones with the charging port facing BACKWARDS
5. Open the patch using MaxMSP. The gyro values should be reflected both in the number boxes and the rotation of the head images.


Troubleshooting:
1. Ensure that the phone and laptop are both connected to the same network
2. Ensure GyrOSC is sending to the correct port (step 2 in the instructions)
3. Ensure GyrOSC is sending to the correct target IP Address (step 2 in the instructions)
	In Windows:
	3.1. Open command prompt
	3.2. Type "ipconfig"
	3.3. Use the IPv4 Address
4. Ensure that GyrOSC is sending gyroscope data (step 3 in the instructions)


![Headtracking Max Patch](https://github.com/bgmennie/JCURA_Max_Headtracking/assets/33833740/6cff3e92-0aac-4b6e-9a48-7938c3bc9791)
