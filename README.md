```tagsearch``` is a small helper script to search recursively through id3 tags in music files.

For my DJ-mixes, I heavily use additional tags to sort my collection, this helps to find files with specific tags on filesystem level.

If you like to listen to some of my Drum & Bass mixes, feel free to visit my artist page: https://hearthis.at/edruskin

### Dependencies:
- ```id3lib```
- ```fd``` (find alternative)

### Installation:
User installation without ```sudo``` requirement

Using git:

```
git clone https://github.com/0xphk/tagsearch.git
```

Set executable bit and copy the script to your preferred users bin directory, which also should be listed in users ```$PATH``` variable.

```sh
cd tagsearch
chmod u+x tagsearch
cp tagsearch ~/bin/
```

### Usage:
```
usage: tagsearch [option] 'search string' ([option] 'search string' ...)
       multiple tags (or based lookup) supported

       tag options: -a artist
                    -b album
                    -c comment
                    -g genre
                    -k key
                    -t title
```

### Notes:
- ```find``` can be used instead of ```fd```
- default result format: ```parent_dir/filename tag: search_result``` (can be changed to full_path or filename only)
- additional tags can be easily added, list available tags using ```id3info filename``` and add option args and condition

### License:
- this is free software, do whatever you like with it

```phk (2022)```
