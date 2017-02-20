===============================================================================
		Software Package - Component
===============================================================================
	1. ReleaseNotes.pdf

	2. document/
		2.1 Quick_Start_Guide_for_Driver_Compilation_and_Installation.pdf
		2.2 Quick_Start_Guide_for_Station_Mode.pdf
		2.3 wpa_cli_with_wpa_supplicant.pdf
		2.4 HowTo_support_more_VidPids.pdf
		2.5 Wireless_tools_porting_guide.pdf
		2.6 HowTo_enable_driver_to_support_WIFI_certification_test.pdf
		2.7 HowTo_enable_the_power_saving_functionality.pdf
		2.8 Quick_Start_Guide_for_SoftAP.pdf
		2.9 SoftAP_Mode_features.pdf
		2.10 linux_dhcp_server_notes.txt
		2.11 Quick_Start_Guide_for_Bridge.pdf
		2.12 RTK_P2P_WFD_Programming_guide.pdf
		2.13 HowTo_enable_driver_to_support_80211d.pdf
		2.14 Realtek_WiFi_concurrent_mode_Introduction.pdf
		2.15 Miracast_for_Realtek_WiFi.pdf
		2.16 Quick_Start_Guide_for_WOW.pdf

	3. driver/
		3.1 rtl8188EUS_linux_v4.3.0.8_13968.20150417.tar.gz
			Naming rule: rtlCHIPS_linux_vM.N.P[.H]_sssss.yyyymmdd[_beta].tar.gz
			where:
				CHIPS: supported chips
				M: Major version
				N: miNor version
				P: Patch number
				H: Hotfix number
				s: SVN number
				y: package year
				m: package month
				d: package day
				_beta: beta driver

	4. wpa_supplicant_hostapd/
		4.1 wpa_supplicant_hostapd-0.8_rtw_r7475.20130812.tar.gz
			4.1.1 wpa_supplicant
				The tool help the wlan network to communicate under the
				protection of WPAPSK mechanism (WPA/WPA2) and add WPS patch
			4.1.2 hostapd
		4.2 wpa_0_8.conf
			 Configure file sample for wpa_supplicant-0.8
		4.3 rtl_hostapd_2G.conf
		4.4 rtl_hostapd_5G.conf
			 Configure files for Soft-AP mode 2.4G/5G
		4.5 p2p_hostapd.conf
			 Configure file for hostapd for Wi-Fi Direct (P2P)

		4.6 wpa_supplicant_8_jb_4.2_rtw_r8680.20130821.tar.gz
			 wpa_supplicant_8 from Android 4.2 SDK and patched by Realtek
			 could be used for pure-linux and Android 4.2. Support only cfg80211/nl80211.

		4.7 wpa_supplicant_8_kk_4.4_rtw_r11967.20140818.tar.gz
			 wpa_supplicant_8 from Android 4.4 SDK and patched by Realtek
			 could be used for pure-linux and Android 4.4. Support only cfg80211/nl80211.

	5. wireless_tools/
		5.1 wireless_tools.30.rtl.tar.gz

	6. WiFi_Direct_User_Interface/
		6.1 p2p_api_test_linux.c
		6.2 p2p_ui_test_linux.c
		6.3 p2p_test.h
		6.4 Start_Guide_P2P_User_Interface_Linux.pdf
	
	7. android_ref_codes_JB_4.2
		7.1 linux-3.0.42_STATION_INFO_ASSOC_REQ_IES.diff
			Kernel patch file for cfg80211's STATION_INFO_ASSOC_REQ_IES event for kernel 3.0.

		7.2 realtek_wifi_SDK_for_android_JB_4.2_20130208.tar.gz
			This tar ball includes our android wifi reference codes for Android 4.2

		7.3 Realtek_Wi-Fi_SDK_for_Android_JB_4.2.pdf
			Guide for porting Realtek wifi onto your Android 4.2 system

	8. android_ref_codes_KK_4.4
		8.1 linux-3.0.42_STATION_INFO_ASSOC_REQ_IES.diff
			Kernel patch file for cfg80211's STATION_INFO_ASSOC_REQ_IES event for kernel 3.0.

		8.2 realtek_wifi_SDK_for_android_KK_4.4_20140117.tar.gz
			This tar ball includes our android wifi reference codes for Android 4.4

		8.3 Realtek_Wi-Fi_SDK_for_Android_KK_4.4.pdf
			Guide for porting Realtek wifi onto your Android 4.4 system

	9. android_ref_codes_L_5.0
		9.1 linux-3.0.42_STATION_INFO_ASSOC_REQ_IES.diff
			Kernel patch file for cfg80211's STATION_INFO_ASSOC_REQ_IES event for kernel 3.0.

		9.2 realtek_wifi_SDK_for_android_L_5.0_20141203.tar.gz
			This tar ball includes our android wifi reference codes for Android 5.0

		9.3 Realtek_Wi-Fi_SDK_for_Android_L_5.0.pdf
			Guide for porting Realtek wifi onto your Android 5.0 system

	10. install.sh
		Script to compile and install WiFi driver easily in PC-Linux

	11. mp_tools/88_89ENormalMPDoc/RF_MP_ToolPackage -20131015.zip
		Document, utilities for MP mode.
		Could be used for EMI tests such as FCC and ETSI tests.

==================================================================================================================
		User Guide for Driver compilation and installation
==================================================================================================================
			(*) Please refer to document/Quick_Start_Guide_for_Driver_Compilation_and_Installation.pdf
==================================================================================================================
		User Guide for Station mode
==================================================================================================================
			(*) Please refer to document/Quick_Start_Guide_for_Station_Mode.pdf
==================================================================================================================
		User Guide for Soft-AP mode
==================================================================================================================
			(*) Please refer to document/Quick_Start_Guide_for_SoftAP.pdf
			(*) Please use wpa_supplicant_hostapd-0.8_rtw_r7475.20130812.tar.gz
			(*) Please refer to document/linux_dhcp_server_notes.txt
==================================================================================================================
		User Guide for Wi-Fi Direct
==================================================================================================================
		Realtek Legacy Wi-Fi Direct:
			(*) Please refer to document/RTK_P2P_WFD_Programming_guide.pdf
			(*) Please use wpa_supplicant_hostapd-0.8_rtw_r7475.20130812.tar.gz
			(*) Please refer to document/linux_dhcp_server_notes.txt
			(*) Please refer to WiFi_Direct_User_Interface/
		Wi-Fi Direct with nl80211
			(*) Please use:
					wpa_supplicant_8_jb_4.2_rtw_r8680.20130821.tar.gz
				or
					wpa_supplicant_8_kk_4.4_rtw_r11967.20140818.tar.gz
			(*) For P2P instruction/command, please refer to:
					README-P2P inside the wpa_supplicant folder of the wpa_supplicant_8 you choose
			(*) For DHCP server, please refer to:
					document/linux_dhcp_server_notes.txt
==================================================================================================================
		User Guide for WPS2.0
==================================================================================================================
			(*) Please use:
					wpa_supplicant_hostapd-0.8_rtw_r7475.20130812.tar.gz
				or
					wpa_supplicant_8_jb_4.2_rtw_r8680.20130821.tar.gz
				or
					wpa_supplicant_8_kk_4.4_rtw_r11967.20140818.tar.gz
			(*) For WPS instruction/command, please refert to:
					README-WPS inside the wpa_supplicant folder of the wpa_supplicant_8 you choose
==================================================================================================================
		User Guide for Power Saving Mode
==================================================================================================================
			(*) Please refer to document/HowTo_enable_the_power_saving_functionality.pdf
==================================================================================================================
		User Guide for Applying Wi-Fi solution onto Andriod System
==================================================================================================================
			(*) For Android 1.6 ~ 2.3, 4.0, 4.1, 4.3, please contact us for further information
			(*) For Android 4.2, please refer to android_ref_codes_JB_4.2/Realtek_Wi-Fi_SDK_for_Android_JB_4.2.pdf
			(*) For Android 4.4, please refer to android_ref_codes_KK_4.4/Realtek_Wi-Fi_SDK_for_Android_KK_4.4.pdf
			(*) For Android 5.0, please refer to android_ref_codes_L_5.0/Realtek_Wi-Fi_SDK_for_Android_L_5.0.pdf
