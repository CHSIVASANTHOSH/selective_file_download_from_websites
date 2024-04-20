# selective_file_download_from_websites
script or command to selectively downlaod the files of larger number  in a website
Here if i want to downlaod files of 100 number but selectively then I use this script or command to downaload where I place the file name  in place of {file names} present in the website to presne tin the script and paste this in the command line .They will automatically get downloaded.
#This will only work for UBUNTU machines

for number in {file names}; do
    wget -r -np -nH --cut-dirs=3 -R index.html "https://www.3gpp.org/ftp/TSG_RAN/WG1_RL1/TSGR1_116b/Docs/$number.zip" -P ~/Downloads
done
