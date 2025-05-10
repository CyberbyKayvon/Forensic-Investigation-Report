# Forensic-Investigation-Report
This project presents a full forensic investigation of a Windows XP system image (`nps-2009-domexusers.E01`) to identify user activity, communication, and file transfer evidence. The analysis was conducted using Autopsy, RegRipper, and manual examination of registry artifacts, prefetch files, email records, and IM logs.

---

## 🎯 Objectives

- Identify user accounts and login activity
- Discover installed software and communication tools
- Analyze recently accessed files and deleted documents
- Investigate email communications and file attachments
- Extract and interpret instant messaging artifacts
- Determine whether sensitive files were sent to remote users

---

## 🔧 Tools & Methods

- **Autopsy**: for image parsing, file carving, artifact extraction
- **RegRipper**: for Windows registry analysis
- **NTUSER.DAT**, **SAM**, **blist.xml**, **prefetch**: key artifact sources
- **Outlook & Thunderbird**: email client data analysis
- **Pidgin Messenger**: for AIM/Jabber logs and buddy lists

---

## 📁 Repo Structure

/forensic-investigation-xp
├── README.md
├── screenshots/
│ └── sam_accounts.png
│ └── pidgin_buddies.png
├── extracted/
│ └── domexuser1_docs/
│ └── email_logs/
├── reports/
│ └── sam_rip.txt
│ └── ntuser_plugins.txt
│ └── prefetch_programs.txt
│ └── communication_summary.txt
└── final_summary.md


---

## 🧠 Key Findings

- **Users Identified**: `domex1` (active), `domex2` (never logged in)
- **Email Evidence**: Multiple emails sent with file attachments (.docx, .xlsx)
- **IM Activity**: Pidgin Messenger logs confirmed active use of AIM and Jabber/XMPP
- **Deleted Files**: Recovered metadata for documents no longer present
- **Program Usage**: Outlook, Firefox, Pidgin, Thunderbird actively used
- **File Transfers**: domex1 sent files to `domexuser2@gmail.com`, `domexuser3@gmail.com`

---

## 🔍 Highlights

- **Emails with attachments**: Word and Excel files sent to outside addresses
- **Buddy list analysis**: IM contacts and aliases suggest regular external communication
- **Prefetch and registry artifacts**: confirm timeline of app usage
- **Autopsy keyword search**: recovered deleted filenames and email strings

---

## 📸 Screenshots

View the `/screenshots` folder for key visuals:
- SAM file user extraction
- Pidgin blist.xml (buddy list)
- Email logs with timestamped attachments

---

## 🛡️ Security Takeaways

- **Communication channels** (email, IM) were active and potentially misused
- **Deleted file artifacts** can still be recovered with proper tools
- Registry and prefetch files are critical in digital forensics
- **User profiling** through artifacts is effective for attribution

---

## 📅 Project Info

- **Student**: Kayvon Karimi  
- **Course**: CYBR-512 – Incident Detection and Handling  
- **Institution**: University of San Diego, Shiley-Marcos School of Engineering  
- **Instructor**: Professor Mark Heckman, Ph.D.  
- **Date**: December 2, 2024

