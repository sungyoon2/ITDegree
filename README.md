# ITDegree
정보보호학위 취득
yoon@sungyoon:~$ sudo openvpn ~/Downloads/starting_point_HophackerYoon.ovpn
2025-06-15 00:57:40 WARNING: Compression for receiving enabled. Compression has been used in the past to break encryption. Sent packets are not compressed unless "allow-compression yes" is also set.
2025-06-15 00:57:40 Note: --data-ciphers-fallback with cipher 'AES-128-CBC' disables data channel offload.
2025-06-15 00:57:40 OpenVPN 2.6.14 x86_64-pc-linux-gnu [SSL (OpenSSL)] [LZO] [LZ4] [EPOLL] [PKCS11] [MH/PKTINFO] [AEAD] [DCO]
2025-06-15 00:57:40 library versions: OpenSSL 3.5.0 8 Apr 2025, LZO 2.10
2025-06-15 00:57:40 DCO version: N/A
2025-06-15 00:57:40 TCP/UDP: Preserving recently used remote address: [AF_INET]154.57.164.105:443
2025-06-15 00:57:40 Socket Buffers: R=[131072->131072] S=[16384->16384]
2025-06-15 00:57:40 Attempting to establish TCP connection with [AF_INET]154.57.164.105:443
2025-06-15 00:57:40 TCP connection established with [AF_INET]154.57.164.105:443
2025-06-15 00:57:40 TCPv4_CLIENT link local: (not bound)
2025-06-15 00:57:40 TCPv4_CLIENT link remote: [AF_INET]154.57.164.105:443
2025-06-15 00:57:41 TLS: Initial packet from [AF_INET]154.57.164.105:443, sid=b0ab0cf2 161910d6
2025-06-15 00:57:41 VERIFY OK: depth=2, C=GR, O=Hack The Box, OU=Systems, CN=HTB VPN: Root Certificate Authority
2025-06-15 00:57:41 VERIFY OK: depth=1, C=GR, O=Hack The Box, OU=Systems, CN=HTB VPN: eu-starting-point-1-dhcp Issuing CA
2025-06-15 00:57:41 VERIFY KU OK
2025-06-15 00:57:41 Validating certificate extended key usage
2025-06-15 00:57:41 ++ Certificate has EKU (str) TLS Web Client Authentication, expects TLS Web Server Authentication
2025-06-15 00:57:41 ++ Certificate has EKU (oid) 1.3.6.1.5.5.7.3.2, expects TLS Web Server Authentication
2025-06-15 00:57:41 ++ Certificate has EKU (str) TLS Web Server Authentication, expects TLS Web Server Authentication
2025-06-15 00:57:41 VERIFY EKU OK
2025-06-15 00:57:41 VERIFY OK: depth=0, C=GR, O=Hack The Box, OU=Systems, CN=eu-starting-point-1-dhcp
2025-06-15 00:57:42 Control Channel: TLSv1.3, cipher TLSv1.3 TLS_AES_256_GCM_SHA384, peer certificate: 256 bits ED25519, signature: ED25519, peer temporary key: 253 bits X25519
2025-06-15 00:57:42 [eu-starting-point-1-dhcp] Peer Connection Initiated with [AF_INET]154.57.164.105:443
2025-06-15 00:57:42 TLS: move_session: dest=TM_ACTIVE src=TM_INITIAL reinit_src=1
2025-06-15 00:57:42 TLS: tls_multi_process: initial untrusted session promoted to trusted
2025-06-15 00:57:43 SENT CONTROL [eu-starting-point-1-dhcp]: 'PUSH_REQUEST' (status=1)
2025-06-15 00:57:43 PUSH: Received control message: 'PUSH_REPLY,route 10.10.10.0 255.255.254.0,route 10.129.0.0 255.255.0.0,route-ipv6 dead:beef::/64,explicit-exit-notify,tun-ipv6,route-gateway 10.10.16.1,topology subnet,ping 10,ping-restart 120,ifconfig-ipv6 dead:beef:4::100c/64 dead:beef:4::1,ifconfig 10.10.16.14 255.255.254.0,peer-id 5,cipher AES-256-CBC,protocol-flags cc-exit tls-ekm dyn-tls-crypt,tun-mtu 1500'
2025-06-15 00:57:43 OPTIONS IMPORT: --explicit-exit-notify can only be used with --proto udp
2025-06-15 00:57:43 OPTIONS IMPORT: --ifconfig/up options modified
2025-06-15 00:57:43 OPTIONS IMPORT: route options modified
2025-06-15 00:57:43 OPTIONS IMPORT: route-related options modified
2025-06-15 00:57:43 OPTIONS IMPORT: tun-mtu set to 1500
2025-06-15 00:57:43 net_route_v4_best_gw query: dst 0.0.0.0
2025-06-15 00:57:43 net_route_v4_best_gw result: via 10.0.2.2 dev eth0
2025-06-15 00:57:43 ROUTE_GATEWAY 10.0.2.2/255.255.255.0 IFACE=eth0 HWADDR=08:00:27:93:17:f5
2025-06-15 00:57:43 GDG6: remote_host_ipv6=n/a
2025-06-15 00:57:43 net_route_v6_best_gw query: dst ::
2025-06-15 00:57:43 net_route_v6_best_gw result: via fe80::2 dev eth0
2025-06-15 00:57:43 ROUTE6_GATEWAY fe80::2 IFACE=eth0
2025-06-15 00:57:43 TUN/TAP device tun0 opened
2025-06-15 00:57:43 net_iface_mtu_set: mtu 1500 for tun0
2025-06-15 00:57:43 net_iface_up: set tun0 up
2025-06-15 00:57:43 net_addr_v4_add: 10.10.16.14/23 dev tun0
2025-06-15 00:57:43 net_iface_mtu_set: mtu 1500 for tun0
2025-06-15 00:57:43 net_iface_up: set tun0 up
2025-06-15 00:57:43 net_addr_v6_add: dead:beef:4::100c/64 dev tun0
2025-06-15 00:57:43 net_route_v4_add: 10.10.10.0/23 via 10.10.16.1 dev [NULL] table 0 metric -1
2025-06-15 00:57:43 net_route_v4_add: 10.129.0.0/16 via 10.10.16.1 dev [NULL] table 0 metric -1
2025-06-15 00:57:43 add_route_ipv6(dead:beef::/64 -> dead:beef:4::1 metric -1) dev tun0
2025-06-15 00:57:43 net_route_v6_add: dead:beef::/64 via :: dev tun0 table 0 metric -1
2025-06-15 00:57:43 Initialization Sequence Completed
2025-06-15 00:57:43 Data Channel: cipher 'AES-256-CBC', auth 'SHA256', peer-id: 5, compression: 'lzo'
2025-06-15 00:57:43 Timers: ping 10, ping-restart 120
2025-06-15 00:57:43 Protocol options: protocol-flags cc-exit tls-ekm dyn-tls-crypt
