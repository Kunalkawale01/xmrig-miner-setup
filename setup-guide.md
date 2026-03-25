# setup-guide

## 1. Create & Download the Repository

- Option A — If you already uploaded to GitHub
```
a. Open your repository in browser
b. Click Code → Download ZIP
c. Extract it anywhere (e.g., Desktop)
```
- Option B — Using Git (recommended)
```
git clone https://github.com/your-username/xmrig-miner-setup.git
cd xmrig-miner-setup
```
## 2. Prepare the Project Folder

After extraction, open the folder:
```
xmrig-miner-setup/
    └── xmrig/
```
Inside, you should see:
```
- xmrig.exe
- config.json
- start.cmd
```
- If Windows blocks ```.exe ``` , allow it (Defender may flag miners).
  
## 3. Edit config.json (IMPORTANT STEP)

- Right-click config.json
- Open with Notepad or VS Code
- Find this section:
```
    "pools": [
     {
    "url": "pool_address:port",
    "user": "your_wallet_address",
    "pass": "x"
    }
    ]
```
Replace:

"url" → your mining pool

Example:
```
pool.supportxmr.com:3333 ---> slow and less crypto mine
or 
gulf.moneroocean.stream:10128 ---> fast and more crypto mine
```
"user" → your wallet address

Example:
```
48A1...yourMoneroWallet
```
✔ Save the file (Ctrl + S)

## 4. Run the Miner

Open Command Prompt 
 ```
Cd "Folder Path"
```
Run:
```
xmrig.exe --config config.json
```
## 5. What You Should See

A terminal window opens showing:

a. CPU info

b. Connection to pool

c. Hashrate like:
 - speed 10s/60s/15m  1200.5 H/s

✔ That means it's working.

## 6. If It Doesn't Work (Common Fixes)

“MSVCR missing” error
- Install:
```Visual C++ Redistributable (x64)```

Blocked by antivirus
- Go to Windows Security
- Add folder to Exclusions

“Connection failed”
- Check pool URL
- Check internet
- Try another pool

## 7. Optional (Performance Tuning)

Inside config.json:

Adjust CPU threads:
```"threads": 4```
Enable huge pages (run CMD as Admin)

- Important Note

Running this will

a. Use high CPU

b. Increase electricity usage

c. Slow your system
