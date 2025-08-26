
# Local DNS Server & Web Hosting Setup using BIND and Apache

As part of my Linux Administration practice, I successfully configured a **DNS server (BIND)** and hosted a website using **Apache** inside a local network (LAN).

## ⚙️ What I Did
- Installed & configured **BIND (named)** service on Linux.  
- Created and deployed a forward zone file `mywebapp.com.fzone` with:
  - **SOA (Start of Authority)** record  
  - **NS (Name Server)** record  
  - **A (Address)** records for root domain & subdomain (www).  
- Updated `/etc/named.conf` with custom zone entry and added **Google & Cloudflare forwarders** for internet access.  
- Validated configuration using:  
  - `named-checkconf`  
  - `named-checkzone mywebapp.com /var/named/mywebapp.com.fzone`  

## 🌐 Testing & Validation
- Verified DNS resolution on Linux with `dig` & `nslookup`.  
- Configured a Windows client to use the DNS server (192.168.234.130).  
- Confirmed that both local domain (**mywebapp.com**) and external domains (e.g., google.com) resolved correctly.  

## 📂 Web Hosting
- Installed & configured **Apache**.  
- Deployed a custom `index.html` page under `/var/www/html/`.  
- Ensured correct permissions and service restart.  
- Successfully accessed the hosted site via browser:  
  - `http://mywebapp.com`  
  - `http://www.mywebapp.com`  

## 🎯 Key Skills Practiced
- Linux Server Administration  
- DNS Management (BIND)  
- Apache Web Server Hosting  
- Network Configuration & Troubleshooting (`dig`, `nslookup`)  
- Cross-platform validation (Linux ↔ Windows)  

## 🚀 Outcome
✅ Successfully deployed a private DNS + website hosting setup inside LAN.  
✅ Learned how to integrate DNS forwarders for seamless **internet + internal domain resolution**.  
✅ Hands-on practice as a **Linux Administrator** managing DNS & Web services.  

---

# 📸 Project Screenshots

## Screenshot 1: Installing BIND
![Screenshot 1](screenshots/1.png)

## Screenshot 2: Configuring named.conf
![Screenshot 2](screenshots/2.png)

## Screenshot 3: Creating Zone File
![Screenshot 3](screenshots/3.png)

## Screenshot 4: Adding SOA & NS Records
![Screenshot 4](screenshots/4.png)

## Screenshot 5: Adding A Records
![Screenshot 5](screenshots/5.png)

## Screenshot 6: Running named-checkconf
![Screenshot 6](screenshots/6.png)

## Screenshot 7: Running named-checkzone
![Screenshot 7](screenshots/7.png)

## Screenshot 8: Testing with dig
![Screenshot 8](screenshots/8.png)

## Screenshot 9: Testing with nslookup
![Screenshot 9](screenshots/9.png)

## Screenshot 10: Windows DNS Setup
![Screenshot 10](screenshots/10.png)

## Screenshot 11: Verifying mywebapp.com on Browser
![Screenshot 11](screenshots/11.png)

## Screenshot 12: Configuring Apache
![Screenshot 12](screenshots/12.png)

## Screenshot 13: Deploying index.html
![Screenshot 13](screenshots/13.png)

## Screenshot 14: Accessing Website via DNS
![Screenshot 14](screenshots/14.png)

## Screenshot 15: Final Working Setup
![Screenshot 15](screenshots/15.png)

---


👉 Connect with me on LinkedIn: [Hareesh Kumar](https://www.linkedin.com/in/hareesh-kumar-02045a339/)
