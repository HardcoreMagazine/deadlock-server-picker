# Deadlock Server Picker
A lightweight server picker for Deadlock. Fork of https://github.com/FN-FAL113/cs2-server-picker

## [Download](https://github.com/HardcoreMagazine/deadlock-server-picker/releases/download/%231/Release.zip)

## ⚙️ Requirements
- Windows 10 or above
- Works on Windows 8.1 but requires [.NET Framework 4.7.2](https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net472-web-installer) to be installed separately.

## ❔FAQ
**1. How it works, will I get banned?!**
 - The app does not modify any game or system files, I can assure you are safe from being banned when using the app as long as you do not download from untrusted sources. It will add necessary firewall policies to block game server relay ip addresses from being accessed by your network thus skipping them in-game when finding a match.

**2. Not being routed to lowest ping server or not working on your location?**
  - Due to the fact that we can only access and block **_IP relay addresses_** from valve's network points around the world rather than the game's actual server IP addresses directly, which are **_not exposed_** publicly, either your connection got relayed to the nearest available server due to **_how Steam Datagram relay works_** or **_your location might be a factor_**. 
- Re-routing can also happen anytime, even mid-game. One of the best ways to test it out is to block low-ping servers and leave out high-ping servers that are far from your current region. If your ping is high in-game, then you are being routed properly, and the blocked IP relays are not able to re-route you to a nearby server. I was able to test this out properly way back.
- Some solutions that might help out but are not guaranteed: turning off any vpn, uninstalling third-party antivirus and let windefender manage the firewall.
- ISP-related issues, such as bad routing or high ping, are out of scope and control since the app only adds firewall entries. Please contact your ISP instead.

**3. Why it requires admin permission on execution?<br>**
  - This is due to how Windows requires elevated execution when adding the necessary firewall policies. If the app is running in normal mode, it will not be able to do its operations and will throw errors.

**4. Windows smartscreen detected unrecognized app/publisher<br>**
  - The app requires a registered publisher which costs a lot of money. Rest assured the app is safe and has been tested already with more than 10k downloads.

**5. I'm receiving frequent timeouts when a match is being confirmed<br>**
  - You may have blocked many servers, for optimal searching and relaying block only the necessary server relays.

**6. Why windows only?<br>**
  - The app is written using VB.NET, and Windows platform still dominates the gaming scene due to better compatibility. [Steam Charts](https://store.steampowered.com/hwsurvey/) has great statistics on this.

**7. Will this work for CS2?**
  - CS2 and Deadlock servers DOES NOT exactly utilize same server relays. Best use original program for that purpose (see link at the top "_Fork of..._").

## 🔽 Disclaimer
- This project or its author are not affiliated, associated, authorized, endorsed by Valve, its affiliates or subsidiaries. Images, names and other form of trademark are registered to their respective owners.
