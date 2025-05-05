# Blockchain
At the begining, I ran the following commands to compare the resualts of both hash_value.py runs
```
$ cd ~/iot/lesson10
$ cat hash_value.py
$ python hash_value.py
$ python hash_value.py
```
The results of both runs are different and don't follow a specific pattern because hashing randomizes outputs.
![CommandLine1](/Images/Blockchain1.png)

## Snakecoin
I ran snakecoin.py which presents an implementation of a blockchain with 20 blocks mined.
```
$ python snakecoin.py
```
![CommandLine1](/Images/Blockchain2.png)
After that, I ran the folllowing command which launches a webpage implementation of a blockchain where blocks can be mined if the "mine" page is accessed:
```
$ python snakecoin-server-full-code.py
```
I opened another terminal, so I can ran the following commands to access the page and mine a block.
```
$ curl "localhost:5000/txion" 
     -H "Content-Type: application/json" 
     -d '{"from": "akjflw", "to":"fjlakdj", "amount": 3}'
$ curl localhost:5000/mine
```
![CommandLine1](/Images/Blockchain3.png)
We can also mine by directly opening the "mine" page.
![CommandLine1](/Images/Blockchain4.png)

## Blockchain App
I ran the following commands to clone the necessary repository:
```
$ git clone https://github.com/satwikkansal/python_blockchain_app.git
$ cd ~/python_blockchain_app
```
Then, I ran these commands to uncomment the last line in the node_server.py file so the server runs at port 8000 and run the node_server.py program.
```
$ nano node_server.py
$ python3 node_server.py
```
I opened another terminal and ran the following command `run_app.py file`.
![CommandLine1](/Images/Blockchain5.png)

I opened up both http://127.0.0.1:8000/mine and http://127.0.0.1:5000/, wrote a message and posted it, requested to mine, and resynced the page.
![CommandLine1](/Images/Blockchain6.png)
