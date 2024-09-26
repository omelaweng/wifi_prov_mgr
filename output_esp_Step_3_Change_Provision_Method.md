I (31) boot: ESP-IDF v5.3-dirty 2nd stage bootloader
I (31) boot: compile time Sep 26 2024 14:21:31
I (31) boot: Multicore bootloader
I (36) boot: chip revision: v3.0
I (40) boot.esp32: SPI Speed      : 40MHz
I (44) boot.esp32: SPI Mode       : DIO
I (49) boot.esp32: SPI Flash Size : 2MB
I (53) boot: Enabling RNG early entropy source...
I (59) boot: Partition Table:
I (62) boot: ## Label            Usage          Type ST Offset   Length
I (70) boot:  0 nvs              WiFi data        01 02 00009000 00006000
I (77) boot:  1 phy_init         RF data          01 01 0000f000 00001000
I (84) boot:  2 factory          factory app      00 00 00010000 00140000
I (92) boot: End of partition table
I (96) esp_image: segment 0: paddr=00010020 vaddr=3f400020 size=2a1e4h (172516) map
I (164) esp_image: segment 1: paddr=0003a20c vaddr=3ffbdb60 size=0571ch ( 22300) load
I (172) esp_image: segment 2: paddr=0003f930 vaddr=40080000 size=006e8h (  1768) load
I (173) esp_image: segment 3: paddr=00040020 vaddr=400d0020 size=a2510h (664848) map
I (406) esp_image: segment 4: paddr=000e2538 vaddr=400806e8 size=15a50h ( 88656) load
I (452) boot: Loaded app from partition at offset 0x10000
I (452) boot: Disabling RNG early entropy source...
I (464) cpu_start: Multicore app
I (473) cpu_start: Pro cpu start user code
I (473) cpu_start: cpu freq: 160000000 Hz
I (473) app_init: Application information:
I (476) app_init: Project name:     wifi_prov_mgr
I (481) app_init: App version:      1
I (485) app_init: Compile time:     Sep 26 2024 14:59:54
I (491) app_init: ELF file SHA256:  1dd481310...
I (497) app_init: ESP-IDF:          v5.3-dirty
I (502) efuse_init: Min chip rev:     v0.0
I (507) efuse_init: Max chip rev:     v3.99 
I (512) efuse_init: Chip rev:         v3.0
I (517) heap_init: Initializing. RAM available for dynamic allocation:
I (524) heap_init: At 3FFAE6E0 len 0000F480 (61 KiB): DRAM
I (530) heap_init: At 3FFC74D0 len 00018B30 (98 KiB): DRAM
I (536) heap_init: At 3FFE0440 len 00003AE0 (14 KiB): D/IRAM
I (542) heap_init: At 3FFE4350 len 0001BCB0 (111 KiB): D/IRAM
I (549) heap_init: At 40096138 len 00009EC8 (39 KiB): IRAM
I (557) spi_flash: detected chip: generic
I (559) spi_flash: flash io: dio
W (563) spi_flash: Detected size(4096k) larger than the size in the binary image header(2048k). Using the size in the binary image header.
I (578) coexist: coex firmware version: dab85ae96
I (583) main_task: Started on CPU0
I (593) main_task: Calling app_main()
I (633) wifi:wifi driver task: 3ffb80e8, prio:23, stack:6656, core=0
I (643) wifi:wifi firmware version: 0caa81945
I (643) wifi:wifi certification version: v7.0
I (643) wifi:config NVS flash: enabled
I (643) wifi:config nano formating: disabled
I (643) wifi:Init data frame dynamic rx buffer num: 32
I (653) wifi:Init static rx mgmt buffer num: 5
I (653) wifi:Init management short buffer num: 32
I (663) wifi:Init dynamic tx buffer num: 32
I (663) wifi:Init static rx buffer size: 1600
I (673) wifi:Init static rx buffer num: 10
I (673) wifi:Init dynamic rx buffer num: 32
I (673) wifi_init: rx ba win: 6
I (683) wifi_init: accept mbox: 6
I (683) wifi_init: tcpip mbox: 32
I (683) wifi_init: udp mbox: 6
I (693) wifi_init: tcp mbox: 6
I (693) wifi_init: tcp tx win: 5760
I (703) wifi_init: tcp rx win: 5760
I (703) wifi_init: tcp mss: 1440
I (703) wifi_init: WiFi IRAM OP enabled
I (713) wifi_init: WiFi RX IRAM OP enabled
I (813) app: button pressed
I (813) app: Starting provisioning
I (823) app: Development mode: using hard coded salt
I (823) app: Development mode: using hard coded verifier
I (823) phy_init: phy_version 4830,54550f7,Jun 20 2024,14:22:08
I (903) wifi:mode : sta (94:b5:55:f6:f5:90)
I (903) wifi:enable tsf
I (913) wifi:mode : sta (94:b5:55:f6:f5:90) + softAP (94:b5:55:f6:f5:91)
I (923) wifi:Total power save buffer number: 16
I (923) wifi:Init max length of beacon: 752/752
I (923) wifi:Init max length of beacon: 752/752
I (933) esp_netif_lwip: DHCP server started on interface WIFI_AP_DEF with IP: 192.168.4.1
I (933) wifi:Total power save buffer number: 16
I (943) esp_netif_lwip: DHCP server started on interface WIFI_AP_DEF with IP: 192.168.4.1
I (953) wifi_prov_mgr: Provisioning started with service name : PROV_F6F590 
I (953) app: Provisioning started
I (963) app: Scan this QR code from the provisioning application for Provisioning.
I (963) QRCODE: Encoding below text with ECC LVL 0 & QR Code Version 10
I (973) QRCODE: {"ver":"v1","name":"PROV_F6F590","username":"wifiprov","pop":"abcd1234","transport":"softap"}
                                          
  █▀▀▀▀▀█ █  ▄▄ ▀▀█▄▄▄█▄▀▀▄▄▀▀  █▀▀▀▀▀█   
  █ ███ █ ██▄ █▄█▄▀▀▀▀▄▀▀█▄▄ ▄█ █ ███ █   
  █ ▀▀▀ █ ▄██ ▀▀▀▀▀  ▄▀█▄▀ ▀█▀  █ ▀▀▀ █   
  ▀▀▀▀▀▀▀ ▀ █▄▀ ▀ █▄▀ ▀▄▀▄▀ ▀▄█ ▀▀▀▀▀▀▀   
  █▀ ▄▀█▀▄ ▄▀ ▀▄ ▄ ▀█▀▄▀██▀▄ ▄▀▄ █▄▀▀▀▀   
  ▀▀ ▀  ▀███▀ ▄ ▀▀█▄  ▄▄▄▀▄ ██▄██ ▀█▄█▄   
  ▄█▄█▀▀▀▀▄▄▄▀▄▄▄█▀██▀▀▀ ▄▀▄ █▀ ▀█▄▀█▄▀   
  ▄▄▄█▀█▀▀▀▄▀█▀ ▄▀██▀▄▀▄██▀▀▄█ █▄█ █▄     
   ▄ ▀█▄▀██ ▄ ▀▄ ▄ ▀█▀▀█ █▀▄▄▄▀██▀▄ ▀▀▀   
  ▄▄ ▄▀▄▀ ▄▀▄ ▄  █▀▄ ▄ █▄▀█ █▀▀█ █▄▀▄▄▄   
  █▀ ▄▀ ▀█ █ ▀▄▄█▄█▀ ▀▀▀ ▄ ▄  ▄██▀▄█▀█▀   
   ▄▄  █▀▄██ █▀▀ ▀██▀ ▀▄█▀ ▀ ▀▀█▄▀ █▄▄▄   
  ▄ ▄ ▀█▀ ██▄ ▀  ▄█▀ ▀▀▀█▄█ ▄▄▀▀█▀▄▀▀ ▀   
     ██ ▀▄▀▀▄ ▄ █▀ ▄ ▄ ██▀ ▀▀▀▀ █▄█▄█▀▄   
  ▀▀▀▀  ▀▀▄█▀▀▄▀██▄▀▄▀██▀█▄▄▄ █▀▀▀█ ▀▄    
  █▀▀▀▀▀█ ▄█ █▀█▀███▄▄ ▄ ▀  ▄▀█ ▀ ██▄     
  █ ███ █ ▀▄█ ▀█▄▄██▄ ▄▀█▄█ ▄▄████▀▄██▄   
  █ ▀▀▀ █ ▄▀▄ ▄ ▄▀▄▄▀▄ ████ █ ▄  ▀▄██▄    
  ▀▀▀▀▀▀▀ ▀▀ ▀ ▀▀ ▀▀ ▀▀▀  ▀  ▀   ▀▀ ▀▀▀   
                                          

I (1243) app: If QR code is not visible, copy paste the below URL in a browser.
https://espressif.github.io/esp-jumpstart/qrcode.html?data={"ver":"v1","name":"PROV_F6F590","username":"wifiprov","pop":"abcd1234","transport":"softap"}
I (22973) wifi:new:<1,0>, old:<1,1>, ap:<1,1>, sta:<0,0>, prof:1, snd_ch_cfg:0x0
I (22973) wifi:station: 4e:81:f3:02:67:56 join, AID=1, bgn, 20
I (22973) app: SoftAP transport: Connected!
I (23193) wifi:<ba-add>idx:2 (ifx:1, 4e:81:f3:02:67:56), tid:0, ssn:0, winSize:64
I (24873) esp_netif_lwip: DHCP server assigned IP to a client, IP is: 192.168.4.2
I (40143) security2: Using salt and verifier to generate public key...
I (40663) app: Secured session established!
I (56393) app: Received Wi-Fi credentials
        SSID     : AIS 4G Hi-Speed Home WiFi_76947550769475
        Password : 50769475
I (60503) wifi:primary chan differ, old=1, new=11, start CSA timer
I (60903) wifi:switch to channel 11
I (60903) wifi:ap channel adjust o:1,1 n:11,2
I (60903) wifi:new:<11,0>, old:<1,0>, ap:<11,2>, sta:<0,0>, prof:1, snd_ch_cfg:0x0
I (60913) wifi:new:<11,2>, old:<11,0>, ap:<11,2>, sta:<11,0>, prof:1, snd_ch_cfg:0x0
I (60923) wifi:state: init -> auth (0xb0)
I (60923) wifi:state: auth -> assoc (0x0)
I (60943) wifi:state: assoc -> run (0x10)
I (60973) wifi:connected with AIS 4G Hi-Speed Home WiFi_769475, aid = 16, channel 11, BW20, bssid = 30:0a:c5:9e:94:9f
I (60973) wifi:security: WPA2-PSK, phy: bgn, rssi: -58
I (61003) wifi:pm start, type: 1

I (61003) wifi:dp: 1, bi: 102400, li: 3, scale listen interval from 307200 us to 307200 us
I (61003) wifi:AP's beacon interval = 102400 us, DTIM period = 1
I (62003) app: Connected with IP Address:192.168.1.119
I (62003) esp_netif_handlers: sta ip: 192.168.1.119, mask: 255.255.255.0, gw: 192.168.1.1
I (62003) wifi_prov_mgr: STA Got IP
I (62013) app: Provisioning successful
I (62013) app: Hello World!
I (62223) wifi:<ba-add>idx:0 (ifx:0, 30:0a:c5:9e:94:9f), tid:0, ssn:4, winSize:64
I (63013) app: Hello World!
I (64013) app: Hello World!
I (65013) app: Hello World!
I (66013) app: Hello World!
I (67013) app: Hello World!
I (67593) wifi:station: 4e:81:f3:02:67:56 leave, AID = 1, reason = 4, bss_flags is 33721443, bss:0x3ffcb3a4
I (67593) wifi:new:<11,0>, old:<11,2>, ap:<11,2>, sta:<11,0>, prof:1, snd_ch_cfg:0x0
I (67593) wifi:<ba-del>idx:2, tid:0
I (67603) wifi:mode : sta (94:b5:55:f6:f5:90)
I (67613) wifi_prov_mgr: Provisioning stopped
I (67613) app: SoftAP transport: Disconnected!
I (68013) app: Hello World!
I (69013) app: Hello World!
I (70013) app: Hello World!
I (71013) app: Hello World!
I (72013) app: Hello World!
I (73013) app: Hello World!
I (74013) app: Hello World!
I (75013) app: Hello World!
I (76013) app: Hello World!
I (77013) app: Hello World!
I (78013) app: Hello World!
I (79013) app: Hello World!
I (80013) app: Hello World!
I (81013) app: Hello World!
I (82013) app: Hello World!
I (83013) app: Hello World!
I (84013) app: Hello World!
I (85013) app: Hello World!
I (86013) app: Hello World!
I (87013) app: Hello World!
I (88013) app: Hello World!
I (89013) app: Hello World!
I (90013) app: Hello World!
I (91013) app: Hello World!
I (92013) app: Hello World!
I (93013) app: Hello World!
I (94013) app: Hello World!
I (95013) app: Hello World!
I (96013) app: Hello World!
I (96843) wifi:<ba-add>idx:1 (ifx:0, 30:0a:c5:9e:94:9f), tid:6, ssn:0, winSize:64
I (97013) app: Hello World!
I (98013) app: Hello World!
I (99013) app: Hello World!
I (100013) app: Hello World!
I (101013) app: Hello World!
I (102013) app: Hello World!
I (103013) app: Hello World!
I (104013) app: Hello World!
I (105013) app: Hello World!
I (106013) app: Hello World!
I (107013) app: Hello World!
I (108013) app: Hello World!
I (109013) app: Hello World!
I (110013) app: Hello World!
I (111013) app: Hello World!
I (112013) app: Hello World!
I (113013) app: Hello World!
I (114013) app: Hello World!
I (115013) app: Hello World!
I (116013) app: Hello World!
I (117013) app: Hello World!
I (118013) app: Hello World!
I (119013) app: Hello World!
I (120013) app: Hello World!
I (121013) app: Hello World!
I (122013) app: Hello World!
I (123013) app: Hello World!
I (124013) app: Hello World!
I (125013) app: Hello World!
I (126013) app: Hello World!
I (127013) app: Hello World!
I (128013) app: Hello World!
I (129013) app: Hello World!
I (130013) app: Hello World!
I (131013) app: Hello World!
I (132013) app: Hello World!
I (133013) app: Hello World!
I (134013) app: Hello World!
I (135013) app: Hello World!
I (136013) app: Hello World!
I (137013) app: Hello World!
I (138013) app: Hello World!
I (139013) app: Hello World!
I (140013) app: Hello World!
I (141013) app: Hello World!
I (142013) app: Hello World!
I (143013) app: Hello World!
I (144013) app: Hello World!
I (145013) app: Hello World!
I (146013) app: Hello World!
I (147013) app: Hello World!
I (148013) app: Hello World!
I (149013) app: Hello World!
I (150013) app: Hello World!
I (151013) app: Hello World!
I (152013) app: Hello World!
I (153013) app: Hello World!
I (154013) app: Hello World!
I (155013) app: Hello World!
I (156013) app: Hello World!
I (157013) app: Hello World!
I (158013) app: Hello World!
I (159013) app: Hello World!
I (160013) app: Hello World!
I (161013) app: Hello World!
I (162013) app: Hello World!
I (163013) app: Hello World!
I (164013) app: Hello World!
I (165013) app: Hello World!
I (166013) app: Hello World!
I (167013) app: Hello World!
I (168013) app: Hello World!
I (169013) app: Hello World!
I (170013) app: Hello World!
I (171013) app: Hello World!
I (172013) app: Hello World!
I (173013) app: Hello World!
I (174013) app: Hello World!
I (175013) app: Hello World!
I (176013) app: Hello World!
I (177013) app: Hello World!
I (178013) app: Hello World!
I (179013) app: Hello World!
I (180013) app: Hello World!
I (181013) app: Hello World!
I (182013) app: Hello World!
I (183013) app: Hello World!
I (184013) app: Hello World!
I (185013) app: Hello World!
I (186013) app: Hello World!
I (187013) app: Hello World!
I (188013) app: Hello World!
I (189013) app: Hello World!
I (190013) app: Hello World!
I (191013) app: Hello World!
I (192013) app: Hello World!
I (193013) app: Hello World!
I (194013) app: Hello World!
I (195013) app: Hello World!
I (196013) app: Hello World!
I (197013) app: Hello World!
I (198013) app: Hello World!
I (199013) app: Hello World!
I (200013) app: Hello World!
I (201013) app: Hello World!
I (202013) app: Hello World!
I (203013) app: Hello World!
I (204013) app: Hello World!
I (205013) app: Hello World!
I (206013) app: Hello World!
I (207013) app: Hello World!
I (208013) app: Hello World!
I (209013) app: Hello World!
I (210013) app: Hello World!
I (211013) app: Hello World!
I (212013) app: Hello World!
I (213013) app: Hello World!
I (214013) app: Hello World!
I (215013) app: Hello World!
I (216013) app: Hello World!
I (217013) app: Hello World!
I (218013) app: Hello World!
I (219013) app: Hello World!
I (220013) app: Hello World!
I (221013) app: Hello World!
I (222013) app: Hello World!
I (223013) app: Hello World!
I (224013) app: Hello World!
I (225013) app: Hello World!
I (226013) app: Hello World!
I (227013) app: Hello World!
I (228013) app: Hello World!
I (229013) app: Hello World!
I (230013) app: Hello World!
I (231013) app: Hello World!
I (232013) app: Hello World!
I (233013) app: Hello World!
I (234013) app: Hello World!
I (235013) app: Hello World!
I (236013) app: Hello World!
I (237013) app: Hello World!
I (238013) app: Hello World!
I (239013) app: Hello World!
I (240013) app: Hello World!
I (241013) app: Hello World!
I (242013) app: Hello World!
I (243013) app: Hello World!
I (244013) app: Hello World!
I (245013) app: Hello World!
I (246013) app: Hello World!
I (247013) app: Hello World!
I (248013) app: Hello World!
I (249013) app: Hello World!
I (250013) app: Hello World!
I (251013) app: Hello World!
I (252013) app: Hello World!
I (253013) app: Hello World!
I (254013) app: Hello World!
I (255013) app: Hello World!
I (256013) app: Hello World!
I (257013) app: Hello World!
I (258013) app: Hello World!
I (259013) app: Hello World!
I (260013) app: Hello World!
I (261013) app: Hello World!
I (262013) app: Hello World!
I (263013) app: Hello World!
I (264013) app: Hello World!
I (265013) app: Hello World!
I (266013) app: Hello World!
I (267013) app: Hello World!
I (268013) app: Hello World!
I (269013) app: Hello World!
I (270013) app: Hello World!
I (271013) app: Hello World!
I (272013) app: Hello World!
I (273013) app: Hello World!
I (274013) app: Hello World!
I (275013) app: Hello World!
I (276013) app: Hello World!
I (277013) app: Hello World!
I (278013) app: Hello World!
I (279013) app: Hello World!
I (280013) app: Hello World!
I (281013) app: Hello World!
I (282013) app: Hello World!
I (283013) app: Hello World!
I (284013) app: Hello World!
I (285013) app: Hello World!
I (286013) app: Hello World!
I (287013) app: Hello World!
I (288013) app: Hello World!
I (289013) app: Hello World!
I (290013) app: Hello World!
I (291013) app: Hello World!
I (292013) app: Hello World!
I (293013) app: Hello World!
I (294013) app: Hello World!
I (295013) app: Hello World!
I (296013) app: Hello World!
I (297013) app: Hello World!
I (298013) app: Hello World!
I (299013) app: Hello World!
I (300013) app: Hello World!
I (301013) app: Hello World!
I (302013) app: Hello World!
I (303013) app: Hello World!
I (304013) app: Hello World!
I (305013) app: Hello World!
I (306013) app: Hello World!
I (307013) app: Hello World!
I (308013) app: Hello World!
I (309013) app: Hello World!
I (310013) app: Hello World!
I (311013) app: Hello World!
I (312013) app: Hello World!
I (313013) app: Hello World!
I (314013) app: Hello World!