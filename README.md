# ASUS-PRIME-B360M-A

OpenCore EFI for ASUS PRIME B360M-A

![about](https://raw.githubusercontent.com/randvmbone/ASUS-PRIME-B360M-A/main/about.png)

### Hardware

* **MOBO:** ASUS PRIME B360M-A
* **CPU:** Intel Core i5-8500
* **RAM:** CORSAIR Vengeance RGB PRO DDR4-3200 16GB (2x8GB)
* **GPU:** ASUS ROG STRIX Radeon RX Vega 64
* **SSD:** Crucial MX500 500GB
* **WIFI:** fenvi FV-T919

### BIOS Settings

* Advanced
	* CPU Configuration
		* Intel VMX Virtualization Technology Enabled → **Enabled**
		* CPU - Power Management Control
			* CFG Lock → **Disabled**  
	*  System Agent (SA) Configuration
		* VT-d  → **Disabled**
		* Graphics Configuration
			* Primary Display → **PEG**
			* iGPU Multi-Monitor → **Disabled**
	* PCH-FW Configuration
		* TPM Device Selection → **Firmware TPM**
	* Onboard Devices Configuration
		* Serial Port Configuration
			* Serial Port  → **Off**
		* Parallel Port Configuration
			* Parallel Port  → **Off**
	* PCI Subsystem Settings
		* Above 4G Decoding → **Enabled**
		* Re-Size BAR Support  → **Enabled**
	* USB Configuration
		* Legacy USB Support → **Enabled**
		* XHCI Hand-off → **Enabled**
* Boot
	* Boot Configuration
		*  Fast Boot → **Disabled**

### macOS Support

| Version   | macOS | Download |
| --------: | :---- | :------- |
| 14.2 | Sonoma | [Mac App Store](https://apps.apple.com/app/macos-sonoma/id6450717509?mt=12) |
| 13.6 | Ventura | [Mac App Store](https://apps.apple.com/app/macos-ventura/id1638787999?mt=12) |
| 12.7 | Monterey | [Mac App Store](https://apps.apple.com/app/macos-monterey/id1576738294?mt=12) |
| 11.7.10 | Big Sur | [Mac App Store](https://apps.apple.com/app/macos-big-sur/id1526878132?mt=12) |
| 10.15.7 | Catalina | [Mac App Store](https://apps.apple.com/app/macos-catalina/id1466841314?mt=12) |
| 10.14.6 | Mojave | [Mac App Store](https://apps.apple.com/app/macos-mojave/id1398502828?mt=12) |
| 10.13.6 | High Sierra | [Mac App Store](https://apps.apple.com/app/macos-high-sierra/id1246284741?mt=12) |

### Sonoma

* OCLP
	* ```boot-args: amfi=0x80 ipc_control_port_options=0```

### Emulate

* Kaby Lake (Required for High Sierra)

  ```Cpuid1Data: E9060900 00000000 00000000 00000000```

  ```Cpuid1Mask: FFFFFFFF 00000000 00000000 00000000```
