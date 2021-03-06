## rss2youtube-dl
A utility that downloads and parses rss feeds for videos to download with youtube-dl  
v.1.0  
2020 by radicalarchivist  

## Usage
    rss2youtube-dl [-CDhid] [-c CONFIGFILE] [-r CHANNEL]
    rss2youtube-dl --help
    rss2youtube-dl --version

    Options:
      -c --config CONFIGFILE                Use custom configuration file             
      -C --cron                             Script being run by cron, don't be interactive.
      -d --demo                             Don't save or add to seen
      -D --debug                            Print debug info to screen.
      -i --interactive                      Interactive mode
      -r --rss-from-channel CHANNEL         Get rss url for youtube channel url provided
      -h --help                             Show this screen
      --version                             Show version info

### Examples

    # Get rss feed address for a youtube channel
    $ rss2youtube-dl -r https://www.youtube.com/user/GoogleDevelopers
    https://www.youtube.com/feeds/videos.xml?channel_id=UC_x5XG1OV2P6uZZ5FSM9Ttw

## .channels.yaml
    example:
        name: Feed Name (required)
        download_dir: /path/to/save/directory (required if not using filter directories)
        rss: https://rss.feed.url.com/.rss (required)
        filter: 
            - "Case Sensitive Filter (title filter)":
                download_dir: /path/to/save/dir (optional)

## Support RadicalArchivist
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N53F7TD)