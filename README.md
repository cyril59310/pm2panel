# pm2panel is web panel for pm2

you can do with this application with web GUI and without any command:

 * Add process to pm2
 * Remove process from pm2
 * Restart process in pm2
 * show log of process in pm2
 * Save processes
 * has login

![](http://4uploader.com/upload/file/201804_1/pm2%20gif5acc753a.gif)

Requirement:

 * nodejs
 * libpam0g-dev (for PAM authentication)

## how use:


```bash
git clone https://github.com/cyril59310/pm2panel
cd pm2panel
npm install
node pm2panel
```

if you have problem in `npm install` step run this command on linux:

On all the Debian/Ubuntu :
```bash
sudo apt-get install libpam0g-dev
sudo apt-get install build-essential
```
On all the Centos and RHEL:
```bash
sudo yum install pam-devel
```


Then you can go to url : http://localhost:1234 or http://server_ip:1234 and the default user is `empty` and password is `empty`.


you can change config in first lines of `config.js`:

```javascript
module.exports = {
    port: 1234,
    pam_auth: false,
    user: "",
    password: "",
}
```

change port or user name and password

<img src="https://www.uplooder.net/img/image/15/fd8d1c8ed2ea1e09e558f423ff2925ae/login-pm2.png" />
<br /><br />
<img src="https://www.uplooder.net/img/image/10/f9f161252a89283a2f5aa85b2b1e1718/pm2index.png" />
