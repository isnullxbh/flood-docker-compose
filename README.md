# flood-docker-compose

Install Flood with Docker Compose

## Getting Started

1. Edit the [compose file](docker-compose.yaml) (UIDs, GIDs, paths)
2. Install rtorrent
3. Run rtorrent as systemd service
4. Compose

**Example (Ubuntu):**

```shell
# Install rtorrent
sudo apt-get install rtorrent

# Run as systemd service
sudo cp rtorrent@.service /etc/systemd/system/
sudo systemctl enable rtorrent@isnullxbh
sudo systemctl start rtorrent@isnullxbh

# Compose
docker compose up --detach
```

## Author

Oleg E. Vorobiov <isnullxbh@gmail.com>
