# buildingdt

Landing page for [www.buildingdt.org](https://www.buildingdt.org).

## Structure

- `index.html` — landing page
- `styles.css` — shared styles (copied from Urban DT repo)
- `*.png` — logos and visuals
- Unity WebGL platform is served separately at `/platform/` (uploaded to server, not in this repo)

## Deploy

The site lives on EC2 at `/var/www/www.buildingdt.org/`. After pushing changes:

```bash
ssh -i ~/Downloads/biorlab.pem ubuntu@47.131.94.3
cd /var/www/www.buildingdt.org
sudo git pull
```

Unity build at `/var/www/www.buildingdt.org/platform/` is updated separately via `scp`.
