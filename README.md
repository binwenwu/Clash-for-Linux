> Clash for Linux Personal Backup Installation Package

### Download && Configure

- *Download project*

```bash
git clone https://github.com/binwenwu/Clash-for-linux.git
```

- *Write proxy and cancel proxy commands into environment variables*

```bash
cat <<EOL >> ~/.bashrc
# Proxy settings
alias proxy='export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890'
alias unproxy='unset https_proxy http_proxy all_proxy'
EOL
```

- *Make environmental variables effective*

```bash
source ~/.bashrc
```

### Usage

- *Enter the project directory*
  - *Place the subscribed configuration file (. yaml) in this directory*

```bash
cd Clash-for-linux
```

- *Set execution permissions*

```bash
chmod +x ./clash-linux-amd64-v1.3.5
```

- *Start program*

```bash
./clash-linux-amd64-v1.3.5 -f ./yourconfig.yaml
```

- *Enable Terminal Agent*

```bash
proxy
```

- *Cancel Terminal Agent*

```bash
unproxy
```

### Notice

- *If `Country.mmdb` is not displayed, Just place `Country.mmdb` in the directory under ``~/. config/clash/``*

```
mkdir -p ~/.config/clash 
cp ./Country.mmdb ~/.config/clash
```

- *Restart the program*

```BASH
./clash-linux-amd64-v1.3.5 -f ./yourconfig.yaml
```
