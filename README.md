> Clash for Linux Personal Backup Installation Package

### Usage

- *Download project*

```bash
git clone https://github.com/binwenwu/Clash-for-linux.git
```

- *Enter the project directory*
  - *Place the subscribed configuration file (. yaml) in this directory*

```bash
cd Clash-for-linux
```

- *Start program*

```bash
./clash-linux-amd64-v1.3.5 -f ./yourconfig.yaml
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

