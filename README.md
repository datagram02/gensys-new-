<div align="center">

# 💻 Gensyn-ai-Rl-Swarm_Guide {Mac/Linux} 💻

</div>


## Device/System Requirements 🖥️

![image](https://github.com/user-attachments/assets/4fbf23bb-846c-4def-be24-157c51fa0b4e)



* Open Your Vps

```
ssh username@ip
```

## Pre-Requirements 🛠

# Install Python and Other Tools

* For **Linux/Wsl**

```
sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl wget screen git lsof

```

Check Version

```
python3 --version
```


# Install Node.js , npm & yarn

* For **Linux/Wsl**

```
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash - && sudo apt update && sudo apt install -y nodejs
```

* Install Yarn (linux)

```
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
```

```
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list > /dev/null
```

```
sudo apt update && sudo apt install -y yarn
```

* Check version **(Linux/Mac)**

```
node -v
```
```
npm -v
```

```
yarn -v
```


<div align="center">

# 👨🏻‍💻 Start The Node (Linux/Mac) 

</div>


 1️⃣ Create a screen session **(vps only)**

```
screen -S gensyn
````


 2️⃣ Clone RL-SWARM Repo

```
git clone https://github.com/gensyn-ai/rl-swarm.git
```


 3️⃣ Navigate to rl-swarm

```
cd rl-swarm
```


* Pull the latest release 


```
git switch main
git reset --hard
git clean -fd
git pull origin main
```




 4️⃣ Create & Activate a Virtual Environment

```
python3 -m venv .venv
source .venv/bin/activate
```


#### 5️⃣ Run the swarm Node 

```
./run_rl_swarm.sh
```


## 5️⃣ Choose customised model's

----> Recommend for Mac 


<pre>

 Gensyn/Qwen2.5-0.5B-Instruct

 Qwen/Qwen3-0.6B

 nvidia/AceInstruct-1.5B

 dnotitia/Smoothie-Qwen3-1.7B

 Gensyn/Qwen2.5-1.5B-Instruct


