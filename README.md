# afterInstall

#I add my config after install linux dest.


#software:
sudo apt update && sudo apt install git mint-meta-codecs vlc audacious docky ffmpeg tlp tlp-rdw keepassxc uget gimp gedit 

#pardus: 
sudo apt update && sudo apt install git ffmpeg tlp tlp-rdw keepassxc uget gimp gedit 



#battery: 
    sudo tlp start

#youtube-dl:
    sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
    sudo chmod a+rx /usr/local/bin/youtube-dl




#Flutter Conf.
#After dowload flutter  :
1- extrac it : tar xf flutter.tar
2- move it where ever want and paste :  export PATH="$PATH:`pwd`/flutter/bin"  

1- extrac it to flutter but it in home 
2- open /etc/environment as root 
and add line below like 
PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/home/medineli/IDE/flutter/bin:/usr/local/android-studio/bin"
FLUTTER="/home/medineli/IDE/flutter/bin"
ANDROID_HOME="/usr/local/android-studio/bin"

dont foget 
1- flutter config --android-sdk /home/medineli/Android/sdk
2- flutter doctor --android-licenses

* install sdk-toolfrom android-studio : Android-SDK> uncheck "Hide OBsolete Pack" , check "Android SDK Tools" &&&&& reboot system






#aliass

#SysTem
alias up='sudo apt update && sudo apt upgrade -y'
alias clean='sudo apt-get autoclean && sudo apt-get clean && sudo apt-get autoremove'
alias install='sudo apt install'
alias remove='sudo apt remove'	


# pythin conda alias
alias sconda='conda config --show | grep auto_activate_base'
alias aconda='conda config --set auto_activate_base True && source ~/.bashrc'
alias dconda='conda config --set auto_activate_base False && source ~/.bashrc'
alias jrun='jupyter-notebook'


# GeeK AliAs
alias ..='cd ..'
alias ...='cd ../../../'
alias ....='cd ../../../../'
alias .....='cd ../../../../'
alias .4='cd ../../../../'
alias .5='cd ../../../../..'


#git 
alias gpush='git add . && git commit -m "first Commit" && git push origin master'

#Network Things
alias ping='ping -c 5'
alias showip='ifconfig'

#Network Things
alias ping='ping -c 5'
alias showip='ifconfig'

# youtube-dl
#audio
alias dlmp3='youtube-dl --no-check-certificate -f "bestaudio/best[height<=480]" --extract-audio --audio-format mp3 -i -o "%(title)s.%(ext)s"'
#one video
alias dloneVideoHigh='youtube-dl --no-check-certificate  -f bestvideo​+bestaudio/best -i -o "%(title)s.%(ext)s"'
alias dloneVideoHighMp4='youtube-dl --no-check-certificate  -f bestvideo​[ext!=webm]‌​+bestaudio/best -i -o "%(title)s.%(ext)s"'
#playList
alias dlsorted-pl='youtube-dl --no-check-certificate  -f bestvideo+bestaudio -i -o "%(playlist_index)s-%(title)s.%(ext)s"'
alias dlsortedBestVideoSound-pl='youtube-dl --no-check-certificate  -f bestvideo+bestaudio/best -i -o "%(playlist_index)s-%(title)s.%(ext)s"'
alias dlsortedHighMp4-pl='youtube-dl --no-check-certificate  -f bestvideo[ext!=webm]‌​+bestaudio/best -i -o "%(playlist_index)s-%(title)s.%(ext)s"'
alias dlhigh-pl='youtube-dl --no-check-certificate  -f bestvideo​+bestaudio/best -i -o "%(title)s.%(ext)s"'
alias dlhighMp4-pl='youtube-dl --no-check-certificate  -f bestvideo[ext!=webm]‌​+bestaudio/best -i -o "%(title)s.%(ext)s"'
