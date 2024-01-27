# FilesCollect-Py

### STATUS
Development. v0.06. ETA <24 hours. Remaining tasks are...
- Final summary stats with completed/failed.
- add additional delays in optimal locations, to purposely not make it the preferred tool for content theifs due to its speed, *ahem ensure processes complete correctly. the idea is to make it easier to download files under circumstances where it is difficult, and time is not the issue, more, effort put in and mental patience, tick tock could be programming etc..guessing the random timer will be, minimum of 15 seconds, then additional random 0-30/60/120/240/480 upon user selection. I'm thinking where huge directories of content in multiple formats for each, it would take about a minimum of 15 seconds to have a good think about something from its title/limited description, if I was actually going to use something before downloading, hyperthetically. 
- testing and bugfixing, ensure am able to get to menu without crash.
- format menu 100% correctly. 
- utils gets bigger than 200 lines, then move download process code to new script ".\scrips\manager.py". 
- check everything over.
- run live tests & bugfix.
- Finish documentation.

## DESCRIPTION
FilesCollect is an advanced web scraping utility designed to streamline the process of collecting files from websites while prioritizing user privacy and convenience. It features an interactive menu that allows users to specify the target URL and file types they wish to download. Leveraging the Tor/Onion network through the Torpy library, FilesCollect offers an enhanced privacy mode for anonymous operations. It ensures a seamless user experience by persistently storing settings in a settings.json file and organizes downloaded files into directories mirroring the URL's structure. With its capability to handle standard and Tor-based web sessions, FilesCollect stands out as a robust and user-friendly tool for efficient web scraping and file management. 

### FEATURES
- **Interactive Menu**: Utilizes an interactive system, enabling users to input the target webpage's URL and specify file extensions.
- **Enhanced Privacy**: Utilizes the Torpy library, offering an optional Tor/Onion network for anonymous, VPN-like downloads.
- **Persistent Settings**: Utilizes a settings.json file for persistent storage and retrieval of user preferences such as base URL and file types.
- **Scraping and Downloading**: Efficiently scrapes web pages for specified file types and downloads files, organizing them in URL-structured directories.
- **Container Extraction**: Generates a unique directory structure for downloaded files based on the webpage's URL, ensuring orderly storage and retrieval.
- **Progress Indication**: Provides real-time progress bars for downloads, active and inactive, full-feature bars, for relevantly, single and threaded, downloads.

### PREVIEW
- Early version (needs updating when its bugfixed)...
```

    print("")
    print("=======================( FilesCollect )=======================")
    print("\n\n\n")
    print("                   1. Content Page Location")
    print(f"{formatted_url}")
    print("")
    print("                    2. File Extension Type")
    print(f"                              ({file_ext_text})")
    print("")
    print("                    3. Network Privacy Modes")
    print(f"                      ({privacy_mode_text})")
    print("")
    print("                      4. Multi-Thread Modes")
    print(f"                      ({asynchronous_mode_4fn_text})")
    print("") 
    print("                      5. Random Timer Delay")
    print(f"                          ({random_delay_r5y})")
    print("")
    print("                      6. Set Tor Port Number")
    print(f"                            ({TOR_PORT})")
    print("\n\n\n")
    print("Select :- Menu Options = 1-6, Begin Scrape = B, Exit Menu = X: ", end='')

```

## USAGE
1. Run `Setup-Install.Bat`, and then, check the libraries all installs correctly and run again as required.
2. Run `FilesCollect-Py.Bat`, and then configure using options 1-3.
3. Press `b` to begin, then watch as the scripts, optionally connect to tor and download the specified files from the specified location.
4. Examine summary screen, determine if all the files were correctly downloaded.
5. Check the `.\Downloads` folder for your files, and then move them to your intended location.    

### REQUIREMENTS
Install is not easy, this will be written further later..
1. Python stuff...
```
pip install requests
pip install beautifulsoup4
pip install torpy
pip install requests[socks]
pip install psutil
pip install asyncio
```
2. Tor Service
```
Download the Tor Expert Bundle: https://www.torproject.org/download/tor/
Extract the Bundle, Run the Tor Service
```
3. Run the program...
```
run FilesCollect-Py.Bat
```


### NOTATION
- After exploring numerous works by a creator, you opt to scrape a selection, and you notice FilesCollect-Py conveniently saves the author's and project's names in the folder name, simplifying future donations. Recognizing the value of the creator's efforts, you plan to contribute financially once you, benefit from their work or have the means.
- This one cannot be done in PowerShell apparemtly, I tried to make it in the first session with powershell and built-in windows 10 functions, but it became impossible. The [torpy](https://pypi.org/project/torpy/) library makes it possible in Python, they get the credit for this project.


## DISCLAIMER
This software is subject to the terms in License.Txt, covering usage, distribution, and modifications. For full details on your rights and obligations, refer to License.Txt.
