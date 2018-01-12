# final_project
NTU Programming Design Final Project of Group 8

<hr>

### 限制

這個目前只有UNIX-like的作業系統能夠編譯、執行，原因是因為socket在windows跟UNIX-like的語法不同，用到的library也不同，所以無法一起編譯。

<hr>

### 編譯

首先因為會用到thread，所以你的電腦必須要有c++11，然後在command line輸入：

'''g++ server.cpp -o server'''

然後會產生一個server的執行檔，接著編譯用戶端：

'''g++ client.cpp -o client -std=c++11'''

會產生一個client的執行檔，因為會用到thread，所以必須加上'''-std=c++11'''。

<hr>

### 執行

'''./server'''
開啟server

'''./client'''
開啟client

<hr>

你必須有六個client連線到server，因為玩家設定是6個人（你也可以在server的程式裡改遊戲人數）。