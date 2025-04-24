# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
## AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.
```
Name   : RAGHUL S
Reg No : 212222040128
```
## DESIGN STEPS:
### Step 1:
Use exiftool to extract metadata from files such as images, documents, and videos.

### Step 2:
Use log2timeline and plaso to create and analyze event timelines from system logs and file metadata.

### Step 3:
Apply steganography detection tools like steghide, zsteg, or binwalk to uncover hidden data in media files.

## PROGRAM:
Metadata and Timeline Forensics, Steganography Analysis Steps

## OUTPUT:
### ✅ A. Using ExifTool – for file metadata
- **📦 Install:**
```bash
sudo apt update
sudo apt install exiftool -y
```
- **📂 Extract metadata from a file:**
```bash
exiftool image.jpg
```
- **📁 Batch process a folder:**
```bash
exiftool -r /path/to/folder
```
- **📌 Useful flags:**
  
- ```-G: Show metadata group```

- ```-time:all: Show only timestamps```

- ```-GPSLatitude -GPSLongitude: Extract GPS data```

  ![6 1](https://github.com/user-attachments/assets/ccce378d-8b3c-4207-a267-30089b7f6e77)


### install log2timeline
```
sudo apt install plaso -y
```

```
sudo apt install steghide -y
```
- **Embed data**
```
steghide embed -cf /home/kali/Downloads/wallpaper.jpg -ef /home/kali/Downloads/secret.txt
```
![6 2](https://github.com/user-attachments/assets/518493c8-0896-483b-a98c-cee123bc6c1f)


- **Extract hidden data:**
```
steghide extract -sf hidden.jpg

```
![6 3](https://github.com/user-attachments/assets/a8e10925-cf1b-474f-aa47-5d17ee7c093f)


### Using binwalk – for file analysis
```bash
sudo apt install binwalk -y
binwalk suspicious.jpg
```
```bash
binwalk /home/kali/Downloads/wallpaper.jpg
```
![6 4](https://github.com/user-attachments/assets/37ab6cc6-a7a7-404d-8acd-1db86684e652)


## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.
