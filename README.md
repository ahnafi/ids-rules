# Rules IDS suricata and snort3

## Installing
As non root
```bash
git clone {this repo}
cd {this repo}
sudo cp snort.lua /usr/local/etc/snort/
sudo cp snortv3/csrf.lua snortv3/sqlinjection.rules snortv3/xss.rules  /usr/local/etc/snort/rules/
```

## Running
As non root
```bash
sudo snort -c /usr/local/etc/snort/snort.lua -i enp0s3
```
once done
```bash
cat /usr/local/etc/snort/alert_json.txt | less
```
