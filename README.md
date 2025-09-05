# Setup-and-Use-a-Firewall-on-Linux (UFW on Linux)

## Objective
Configure and test basic firewall rules to allow or block traffic.

### Steps Performed
1. Checked firewall status:
```
sudo ufw status numbered
```
3. Allowed SSH:
```
sudo ufw allow 22
```
3. Enabled UFW: 
```
sudo ufw enable
```
4. Blocked Telnet (port 23):
```   
sudo ufw deny 23
```
5. Tested rule with Telnet — connection failed.
```
telnet <your_ip> 23
```
6. Removed the test rule:
```
sudo ufw delete <rule_number>
```
 #### Summary
UFW was enabled and configured to block Telnet while allowing SSH. Rule removal restored the original firewall state.

Screenshots:
<img width="628" height="305" alt="ufw_enable" src="https://github.com/user-attachments/assets/b33df76e-c28e-4b35-bdbb-17af57a43c63" />
<img width="646" height="382" alt="delete_rule" src="https://github.com/user-attachments/assets/e889e8f1-9931-4f7f-adfd-a33d060263cb" />


