Contributor: @flyingrub/scdl
https://github.com/flyingrub/scdl/tree/master
Installation instructions: https://github.com/flyingrub/scdl/wiki/Installation-Instruction

Mike Lucarelli
https://www.youtube.com/watch?v=6ebIKw4OnEI&t=1s

Nguyen Tien Dat

Hi everyone! I was tasked by my supervisor to download a bunch of audiobooks from https://radiotoday.net/audio-book as they need them for Viet-ASR (Automatic Speech Recognition) work. At first, I started manually downloading the mp3 files like an idiot. I’m glad I stopped after downloading a playlist and asked him how many he needed. He suggested using a crawler to make it more efficient and faster. So I searched around and found a scdl GitHub code by flyingrub. I followed all the instructions and they worked perfectly on PyCharm. When I started downloading however, mp3 files are downloaded but when I opened them, a weird looking text file came up despite it being mp3 format. Since it did not work for me, I went and watch a Youtube video by Mike Lucarelli where he only used the command prompt. 
Step 1: Install Python 3.7 
Step 2: Open command prompt and type: pip3 install scdl
Step 3: Make sure you have ffmpeg installed (this is argubly the most challenging step) but I used https://www.youtube.com/watch?v=IECI72XEox0&t=360s by TroubleChute. 
Step 4: Depends on what artists, tracks, playlists you want to download, use these. 
If scdl command is not found, use: python3 -m scdl.scdl -l <link>

# Download track & repost of the user QUANTA
scdl -l https://soundcloud.com/quanta-uk -a

# Download likes of the user Blastoyz
scdl -l https://soundcloud.com/kobiblastoyz -f

# Download one track
scdl -l https://soundcloud.com/jumpstreetpsy/low-extender

# Download one playlist
scdl -l https://soundcloud.com/pandadub/sets/the-lost-ship

# Download only new tracks from a playlist
scdl -l https://soundcloud.com/pandadub/sets/the-lost-ship --download-archive archive.txt -c

# Sync playlist
scdl -l https://soundcloud.com/pandadub/sets/the-lost-ship --sync archive.txt

# Download your likes (with authentification token)
scdl me -f

These links works fine. However, downloading is a pain. For example, I need to download audiobooks in mp3 format and I found out the channel has 5642 tracks in total. Assuming an average track size of 5 MB, and an internet connection speed of 50 Mbps, it would take approximately 18.8 hours to download all 5642 tracks. Hence, It is better to do this on a company server so your laptop do not run out of storage and memory. Thank you for reading and do reach out to me (tiendat311003@gmail.com) if you have any information!


