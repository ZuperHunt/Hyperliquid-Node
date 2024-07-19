![image](https://github.com/user-attachments/assets/004ca2d0-5e6c-4c2e-937c-e3457565e88e)

Penulis: [Naufal](https://x.com/0xfal)

> [!NOTE]
> **WHAT IS Hyperliquid?**\
> ..

# Tutorial Hyperliquid Node

## Needs

### Computer

You can use either VPS or your local PC with requirements:

| ✅ Linux (Ubuntu 24.04) |
| ------------- |

| Part | Minimum | Recommended |
| ------------- | ------------- | ------------- |
| CPU | - | 4 Core |
| RAM | - | 16 GB |
| SSD | - | 50 GB |

## Run Node

### Create a non-root User

```
sudo adduser zuperliquid
sudo usermod -aG sudo zuperliquid
su - zuperliquid
```

### Setup

```
curl https://binaries.hyperliquid.xyz/Testnet/initial_peers.json > ~/initial_peers.json
echo '{"chain": "Testnet"}' > ~/visor.json
curl https://binaries.hyperliquid.xyz/Testnet/non_validator_config.json > ~/non_validator_config.json
curl https://binaries.hyperliquid.xyz/Testnet/hl-visor > ~/hl-visor && chmod a+x ~/hl-visor
```

### Create tmux

```
tmux
```

### Running

```
~/hl-visor
```

# Help

## How to detach from tmux session?

Press `ctrl` + `b` + `d` on your keyboard

## How to attach to last tmux session?

Run following command:
```
tmux a
```

---

Reach us if you have more questions:\
ZuperHunt's [Discord server](https://discord.gg/ZuperHunt) | [X(Twitter)](https://twitter.com/ZuperHunt)

# Acknowledgements

* [Hyperliquid](https://github.com/hyperliquid-dex/node)
* [tmux cheatsheet](https://quickref.me/tmux.html)
