
<style>
* {
    box-sizing: border-box;
}
.row::after {
    content: "";
    clear: both;
    display: table;
}
[class*="col-"] {
    float: left;
    padding: 15px;
}
html {
    font-family: "Lucida Sans", sans-serif;
}
.header {
    background-color: #000;
    color: #ffffff;
    padding: 5px;
}
.menu ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}

a{
	  font-family: "Lucida Sans", sans-serif;
	  text-decoration: none;
	  color: #fff;

}

.menu  li  {
    padding: 4px;
    margin-bottom: 7px;
    background-color: #f00;
    color: #ffffff;
    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
    text-decoration: none;
}
.menu li:hover {
    background-color: #000;
}
.aside {
    background-color: #0099cc;
    padding: 15px;
    color: #ffffff;
    text-align: left;
    font-size: 14px;
    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}
.footer {
    background-color: #0099cc;
    color: #ffffff;
    text-align: center;
    font-size: 12px;
    padding: 15px;
}
/* For mobile phones: */
[class*="col-"] {
    width: 100%;
}
@media only screen and (min-width: 768px) {
    /* For desktop: */
    .col-1 {width: 8.33%;}
    .col-2 {width: 16.66%;}
    .col-3 {width: 25%;}
    .col-4 {width: 33.33%;}
    .col-5 {width: 41.66%;}
    .col-6 {width: 50%;}
    .col-7 {width: 58.33%;}
    .col-8 {width: 66.66%;}
    .col-9 {width: 75%;}
    .col-10 {width: 83.33%;}
    .col-11 {width: 91.66%;}
    .col-12 {width: 100%;}
}

</style>
<body>
# rpi
rpi code and configuration
<pre>
Updated 
As root (sudo -i)

# useradd -m -d /home/username  username
# usermod -a -G pi,adm,dialout,cdrom,sudo,audio,video,plugdev,games,users,input,netdev,gpio,i2c,spi cwc

# apt-get upgrade
# apt-get update
// optional
# dpkg --configure -a
#apt-get autoremove

#apt-get install firefox-esr
#apt-get install bless

// nodejs
curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -
sudo apt-get install -y nodejs


</pre>


</body
