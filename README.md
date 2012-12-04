hastebin-python-client
======================

Python 2.x client for hastebin.

Original source from peterbe.com:
www.peterbe.com/plog/hastebinit

## Installation
``` bash
wget https://raw.github.com/tripflex/hastebin-python-client/master/haste
mv haste ~/bin/haste
chmod +x ~/bin/haste
```

## Usage
``` bash
cat ~/myfile | haste
haste < ~/myfile
haste ~/myfile myotherfile
```

## Troubleshooting
If you get a "haste: command not found" you need to set the correct path. In installation above we installed into ~/bin/haste

Check path with this command and make sure the file is in one of those directories:
``` bash
echo ${PATH}
```

If not you can export path to your .bashrc file
``` bash
PATH=~/bin:"${PATH}"
export PATH
```

And verify
``` bash
which haste
```
