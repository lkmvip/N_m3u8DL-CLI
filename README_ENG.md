```

███╗   ██╗        ███╗   ███╗██████╗ ██╗   ██╗ █████╗ ██████╗ ██╗       ██████╗██╗     ██╗
████╗  ██║        ████╗ ████║╚════██╗██║   ██║██╔══██╗██╔══██╗██║      ██╔════╝██║     ██║
██╔██╗ ██║        ██╔████╔██║ █████╔╝██║   ██║╚█████╔╝██║  ██║██║█████╗██║     ██║     ██║
██║╚██╗██║        ██║╚██╔╝██║ ╚═══██╗██║   ██║██╔══██╗██║  ██║██║╚════╝██║     ██║     ██║
██║ ╚████║███████╗██║ ╚═╝ ██║██████╔╝╚██████╔╝╚█████╔╝██████╔╝███████╗ ╚██████╗███████╗██║
╚═╝  ╚═══╝╚══════╝╚═╝     ╚═╝╚═════╝  ╚═════╝  ╚════╝ ╚═════╝ ╚══════╝  ╚═════╝╚══════╝╚═╝
                                                                                          
```
This is a m3u8 downloader.  
## Summary
Supports: 
  * Auto deceypt for `AES-128`
  * `Master List`
  * Live stream recording(`BETA`)
  * `Dolby Vision` from IQiYi, YouKu, Tencent
  * Customize HTTP headers
  * Auto merge clips(Binary or ffmpeg)
  * Select save clip by `time code` or `index`
  * Network driver on Windows OS
  * Alternative audio/video track
  * Mux without video track
  * Auto use system proxy
  * Optimization for Chinese streaming platform
  
  ![ScreenShot](https://nilaoda.github.io/N_m3u8DL-CLI/source/images/%E7%9B%B4%E6%8E%A5%E4%BD%BF%E7%94%A8.gif)  
  
## GUI
  * Easy-to-use `GUI`
  
## Options
```
N_m3u8DL-CLI.exe <URL|JSON|FILE> [OPTIONS]  

    --workDir    Directory      Set work dir (Video will be here)
    --saveName   Filename       Set save name(Exclude extention)
    --baseUrl    BaseUrl        Set Baseurl
    --headers    headers        Set HTTP headers，format: key:value user | split all key&value
    --maxThreads Thread         Set max thread(default: 32)
    --minThreads Thread         Set min thread(default: 16)
    --retryCount Count          Set retry times(default: 15)
    --timeOut    Sec            Set timeout for http request(second，default: 10)
    --muxSetJson File           Set a json file for mux
    --useKeyFile File           Use 16 bytes file as KEY for AES-128 decryption
    --useKeyBase64 Base64String Use Base64 String as KEY for AES-128 decryption
    --downloadRange Range       Set range for a video
    --stopSpeed  Number         Speed below this, retry(KB/s)
    --maxSpeed   Number         Set max download speed(KB/s)
    --enableDelAfterDone        Enable delete clips after download completed
    --enableMuxFastStart        Enable fast start for mp4
    --enableBinaryMerge         Enable use binary merge instead ffmpeg
    --enableParseOnly           Enable parse mode
    --enableAudioOnly           Enable only audio track when mux use ffmpeg
    --disableDateInfo           Disable write date info when mux use ffmpeg
    --noMerge                   Disable auto merge
    --noProxy                   Disable use system proxy
    --disableIntegrityCheck     Disable integrity check
```
  
## Document
  https://nilaoda.github.io/N_m3u8DL-CLI/
