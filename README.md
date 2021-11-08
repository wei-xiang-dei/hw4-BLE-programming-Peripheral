# hw4-BLE-programming-Peripheral


## set up
1,先把https://os.mbed.com/teams/mbed-os-examples/code/mbed-os-example-ble-Button/ 的檔案import到mbed os
2,裡頭的main.cpp 和 pretty_printer.h 用這個github的檔案取代，跟c++相關的其他檔案也import到source裡面
3,準備樹梅派，並在樹莓派環境裝好bluepy套件用來執行Ble_new.py用

## run code
1,注意樹梅派裡頭BLE_new.py裡頭的31行，裡面的字串換成所要連的gatt server的藍芽mac位址，還有gatt server的位置特性(random或public)
2,先在mbed按執行之後，就可以讓stm32扮演gatt server的角色，再用樹梅派的ble.py來去獲取需要的服務，我們寫的是可以讓原本板子上不亮的led再執行後變成亮，達到peripheral控制led的效果


## reference

https://os.mbed.com/teams/mbed-os-examples/code/mbed-os-example-ble-LED/ 


