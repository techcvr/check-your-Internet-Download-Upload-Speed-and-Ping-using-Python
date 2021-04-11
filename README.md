# check-your-Internet-Download-Upload-Speed-and-Ping-using-Python

Python can also be used for testing Internet speed. Python provides different types of libraries for doing the same. There is a library called speedtest-cli. This library is a command-line interface for testing internet bandwidth using speedtest.net

### Installation
This module does not come built-in with Python. To install it type the below command in the terminal.
```Python
pip install speedtest-cli 
```
After installing the literary copy the code given below and test it.

### CODE
```Python
import speedtest
st = speedtest.Speedtest()
option = int(input('''What speed do you want to test:
1) Download Speed
2) Upload Speed
3) Ping
Your Choice: '''))

if option == 1:
    print(st.download(), 'b/s')
if option == 2:
    print(st.upload(), 'b/s')
if option == 3:
    servernames =[]
    st.get_servers(servernames)
    print(st.results.ping, 'b/s')
else:
    print("Please enter the correct choice !")
```
### OUTPUT
```html
What speed do you want to test:
1) Download Speed
2) Upload Speed
3) Ping
Your Choice: 1
15324931.568396978 b/s

What speed do you want to test:
1) Download Speed
2) Upload Speed
3) Ping
Your Choice: 2
2813118.9732526364 b/s
```
I searched for many tutorials but this one is the simple and best.
