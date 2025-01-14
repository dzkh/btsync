BitTorrent Sync was a proprietary peer-to-peer file synchronization tool available for Windows, Mac, Linux, Android, iOS, Windows Phone, Amazon Kindle Fire and FreeBSD.
Transport protocol: https://github.com/arvidn/libtorrent
Every DPI system detects such traffic with no issues. There is no secret data channels for ministro del coca and cia 😁

- 1.3 - classic version without links support. Preferable to use in close environments. This version will probably out of support by tracker and the only way to find remote peer in this case is known hosts.
- 1.4.111+ - They established Resilio Inc. after ending coop with Bittorrent as RnD. Added sharing via links and rewritten internals.
- 2.0.x - this is selective sync verion. Every sharing request can be approved,single file can be shared. Request-approval are unstable in any DPI-enabled network plus relies on external services. Can be turned off and should.

**MacOs**
  
Os may detect app as malware. However no engines on Virustotal (7d38b81cf0ef553dd1f67f719e6e21ba4f745723ccb905c668470e44104caf56) were able to find something and thus the only issue here is a Mac OS Gatekeeper.
As of my own opinion malware exists in builds from 2016. Permissions requested are equal to permissions needed by ReiKey. ReiKey used to detect keyloggers. But maybe they control hotkeys that way?

![Screenshot 2025-01-14 at 10 39 42](https://github.com/user-attachments/assets/dce9e329-3a13-4cab-bd49-4a679ba7fc07)

![Screenshot 2025-01-14 at 01 12 14](https://github.com/user-attachments/assets/0ebd564d-5526-4973-b52d-e5fa589bd68f)

- To solve that you can create new self-signed cert then resign app & components using simple syntax: codesign -s "cert-name-in-Keychain" -f --timestamp -o runtime -i com.bittorrent.Sync BitTorrent\ Sync.app/Contents/MacOS/BitTorrent\ Sync.
- Additionally you can strip i386 binary to decrease file size: lipo -remove i386 BitTorrent\ Sync -output btsync.
- The Gatekeeper probably needs to be disabled.

**Linux**
  
For 1.3 and 1.4 it wasn't planned to support glibc 2.3 enlarged Linux'es. Do not expect stable operation with that builds.
Glibc shipped that days by the distros maintainers was 2.x and no one never added glibc 2.3 to stable updates channel: https://unix.stackexchange.com/questions/224255/upgrading-ubuntu-14-04-to-glibc-2-20-or-greater

Reason they published glibc_2.3 builds of Bittorent Sync was (and still) unknown.

As a proof: listing of publicly availble glibc sources on gnu.org: https://ftp.gnu.org/gnu/glibc/
![image](https://github.com/user-attachments/assets/53bd01f8-642e-4fb5-9aaa-956a8295d1e4)


**FreeBSD**
  
Since inotify-like subsystem wasn't available the only notification about changes in files you sharing is folderRescanInterval. Should be nice for big files & huge folderRescanInterval.
