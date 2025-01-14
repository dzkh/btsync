BitTorrent Sync was a proprietary peer-to-peer file synchronization tool available for Windows, Mac, Linux, Android, iOS, Windows Phone, Amazon Kindle Fire and FreeBSD. Transport protocol: https://github.com/arvidn/libtorrent
Every DPI system detects such traffic with no issues. There is no secret data channels for ministro del coca and cia 😁

- 1.3 - classic version without links support. Preferable to use in close environments. This version will probably out of support by tracker and the only way to find remote peer in this case is known hosts.
- 1.4.x - They established Resilio Inc. using forked sources. Added sharing via links and rewritten internals.
- 2.0.x - this is selective sync verion. Every sharing request can be approved,single file can be shared. Request-approval are unstable in any DPI-enabled network plus relies on external services. Can be turned off and should.

**MacOs**
Os may detect app as malware.
![Screenshot 2025-01-14 at 01 12 14](https://github.com/user-attachments/assets/0ebd564d-5526-4973-b52d-e5fa589bd68f)
However no engines on Virustotal (7d38b81cf0ef553dd1f67f719e6e21ba4f745723ccb905c668470e44104caf56) were able to find something and thus the only issue here is a Mac OS Gatekeeper.
As of my own opinion malware exists in builds from 2016. Permissions requested are equal to permissions needed by ReiKey. ReiKey used to detect keyloggers. But maybe they control hotkeys that way?

To solve that you can create new self-signed cert then resign app components using simple syntax: codesign -s "Dmitriy Khmelkov" -f --timestamp -o runtime -i com.bittorrent.Sync BitTorrent\ Sync.app/Contents/MacOS/BitTorrent\ Sync
Additionally you can strip i386 binary to decrease file size: lipo -remove i386 BitTorrent\ Sync -output btsync

**Linux**
For 1.3 and 1.4 it wasn't planned to support i386, x86_64 with old glibc. Do not expect that.
