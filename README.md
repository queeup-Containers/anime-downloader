# anime-downloader

**[anime-downloader](https://github.com/anime-dl/anime-downloader) in a container**

**_Pull from docker.io:_**
```
$ docker pull queeup/anime-downloader
```

**_Pull from ghcr.io:_**
```
$ docker pull ghcr.io/queeup/anime-downloader
```

**_Volumes:_**
 - `-v config:/config`
 - `-v download:/download`

**_Example usage:_**
```bash
docker run --rm --network=host -ti \
    -v ~/anime:/downloads \
    -v ~/anime/.config:/config \
    queeup/anime-downloader:git --help
````

*Note:* You can use `aria2.conf`file (*you have to create yourself*) for changing your aria2 options on your config directory.

