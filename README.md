# GPIO-PIN-access from terminal in Dragonboard 410c
1. Connect your dragon board with your MAC/PC (Make sure, you have Android Studio installed)<br />
2. Change the directory to platform-tools. As an example: <br />
```
cd Library/Android/sdk/platform-tools/ 
```
3. Check Dragon board is connected or not by using command below: 
```
adb devices
```
You will see output like this: <br />
List of devices attached <br />
82cf2e50	device
4. If the your board is on the list above, enter to the Dragon Board shell:  <br />
```
adb shell

```
Now you will see that you are in device shell terminal and look like this: <br />
shell@msm8916_64:/ $ 
5. Now we need super user access, to get that type below command to become super user: <br />
```
su
```
6. Enter to the sys directory :<br />
```
cd sys
```
7. Enter to the class directory: <br />
```
 cd class
 ```
 8. Now enter to gpio directory: <br />
 ```
 cd gpio
 ```
 9. Type 'ls' to see the the gpio chip. It should look like below:  <br />
 export <br />
gpiochip576 <br />
gpiochip608 <br />
gpiochip640 <br />
gpiochip672 <br />
gpiochip704 <br />
gpiochip736 <br />
gpiochip768 <br />
gpiochip800 <br />
gpiochip832 <br />
gpiochip864 <br />
gpiochip896 <br />
gpiochip900 <br />
gpiochip902 <br />
unexport <br />
10. Enter any of the directory, example: <br />
```
cd gpiochip902
```
11. Type ls to see all about that chip. <br />
