# Cara Memulai Ethical Hacking untuk Pemula

> 📅 2026-05-25 | ✍️ Moyo Attacker | 🏷️ Ethical Hacking, Pemula

![Ethical Hacking](https://images.unsplash.com/photo-1550751827-4bd374c3f58b?w=800)

## Apa itu Ethical Hacking?

**Ethical hacking** (atau white-hat hacking) adalah praktik menguji keamanan sistem komputer, jaringan, atau aplikasi **dengan izin** dari pemiliknya. Tujuannya adalah menemukan celah keamanan sebelum dieksploitasi oleh hacker jahat (black-hat).

> 🔐 "To catch a thief, you must think like a thief" - Keamanan siber bekerja dengan prinsip yang sama.

---

## Perbedaan Jenis Hacker

| Jenis | Motivasi | Legal? |
|-------|----------|--------|
| **White Hat** | Melindungi, mencari celah untuk diperbaiki | ✅ Legal (dengan izin) |
| **Black Hat** | Keuntungan pribadi, merusak | ❌ Ilegal |
| **Grey Hat** | Iseng, mencari celah tanpa izin tapi tidak merusak | ⚠️ Abu-abu |

---

## Langkah Awal Belajar Ethical Hacking

### 1. Pelajari Dasar-Dasar Jaringan Komputer

Pahami konsep-konsep berikut:
- **TCP/IP** - Protokol dasar internet
- **DNS** - Domain Name System
- **HTTP/HTTPS** - Protokol web
- **Subnetting** - Pembagian jaringan
- **Port dan Protocol** (Port 80, 443, 22, dll)

### 2. Kuasai Sistem Operasi Linux

Linux adalah OS utama untuk security testing. Mulai dengan:
```bash
# Perintah dasar Linux yang wajib tahu
ls -la          # Melihat daftar file
cd /etc         # Pindah direktori
sudo apt update # Update package
chmod +x file   # Memberi izin eksekusi
```
Distro yang direkomendasikan:

Ubuntu - Untuk pemula

Kali Linux - Untuk security testing (sudah banyak tools)

Parrot OS - Alternatif ringan

3. Pelajari Bahasa Scripting
Python adalah pilihan terbaik untuk pemula:

python
# Contoh script sederhana untuk scanning port
import socket

def scan_port(host, port):
    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
    sock.settimeout(1)
    result = sock.connect_ex((host, port))
    sock.close()
    return result == 0

# Scan port 80 dan 443
for port in [80, 443, 22]:
    if scan_port("google.com", port):
        print(f"Port {port} terbuka!")
4. Kenali Tools Keamanan Dasar
Tool	Fungsi
Nmap	Network scanning, port scanning
Wireshark	Packet analysis
Burp Suite	Web security testing
Metasploit	Exploitation framework
John the Ripper	Password cracking
5. Praktik di Platform Legal
Jangan pernah testing ke sistem orang tanpa izin! Gunakan platform ini:

HackTheBox - Lab CTF profesional

TryHackMe - Tutorial interaktif untuk pemula

PentesterLab - Fokus web security

OverTheWire - Game wargame untuk belajar command line

Sertifikasi yang Diakui Industri
Setelah mahir, incar sertifikasi ini:

CEH (Certified Ethical Hacker) - EC-Council

OSCP (Offensive Security Certified Professional) - Paling dihormati

CompTIA Security+ - Untuk fundamental

GPEN (GIAC Penetration Tester) - SANS

Etika yang Harus Dipegang
text
1. ❌ Jangan pernah testing tanpa izin tertulis
2. ✅ Laporkan celah yang ditemukan secara bertanggung jawab
3. ❌ Jangan merusak atau mencuri data
4. ✅ Gunakan ilmu untuk melindungi, bukan menyerang
5. ❌ Jangan membagikan exploit ke publik tanpa koordinasi vendor
Mulai Sekarang! 🚀
Roadmap 30 hari untuk pemula:

Hari	Topik
1-7	Dasar jaringan & Linux
8-14	Belajar Python untuk security
15-21	Main-main dengan Nmap & Wireshark
22-30	Coba CTF di TryHackMe
Sumber Belajar Gratis
📚 OWASP Top 10 - 10 celah web terbesar

🎥 The Cyber Mentor - YouTube

📖 Hacker101 - Dari tim HackerOne

🎮 PicoCTF - CTF untuk pelajar

💡 Pesan penting: Ethical hacking adalah tentang melindungi, bukan merusak. Gunakan skillmu untuk kebaikan dan selalu hormati hukum yang berlaku.

