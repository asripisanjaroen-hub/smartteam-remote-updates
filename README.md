# SmartTeam Remote updates

[Download the latest Windows EXE](https://github.com/asripisanjaroen-hub/smartteam-remote-updates/releases/latest)

This repository distributes the Windows program and its signed update manifest. Application source is maintained in a separate private repository. Release assets here contain only the EXE and smartteam-latest.json; no source archive, credentials or user data are published here.

## อัปเดตโปรแกรม

รุ่นใหม่ตรวจ GitHub เมื่อเริ่มและทุก 5 นาที โดยไม่ต้องล็อกอินหรือใส่ token เมื่อพบรุ่นใหม่ กดปุ่มอัปเดตแล้วเลือกติดตั้ง การติดตั้งจะปิดการรีโมตที่กำลังใช้อยู่ ชื่อเครื่องและรายชื่อเดิมยังอยู่

เครื่อง v26.22 ใช้ประกาศอัปเดตเดิมเป็นทางย้ายรุ่น เมื่อเปิดสะพานแล้ว เปิดโปรแกรมใหม่หรือคลิกขวา tray → ตรวจอัปเดต → อัปเดตและเปิดโปรแกรม ไม่ต้องถอนติดตั้ง รุ่น v26.23–v26.25 ที่ยังไม่มีสิทธิ์ GitHub ให้เปิด EXE ล่าสุดจากหน้านี้ครั้งแรก

The updater verifies the existing publisher RSA signature, package SHA256, size and assembly version before installation. Downloading the program does not authorize access to another computer; remote access still requires the host's consent or configured password. Screen sharing uses your LAN or private Tailscale network.

## FFmpeg notice

The EXE embeds an independent FFmpeg 9.0.1 essentials build from gyan.dev, licensed under GPL v3. FFmpeg and its license, build configuration and notices are extracted on first use under LocalAppData/SmartTeamRemote. [Corresponding FFmpeg source revision](https://github.com/FFmpeg/FFmpeg/commit/bf1b838f2a), [Windows build provider](https://www.gyan.dev/ffmpeg/builds/), [GPL v3 license](https://www.gnu.org/licenses/gpl-3.0.html).