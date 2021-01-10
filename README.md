# git-sed

## how to use
``` bash
git-sed 's/double/float/g' ':*.cpp'
git-fixedsed '/root' '/user/hoge' ':*.cpp'
```

### output example
``` bash
$ git-sed 's/emoji:/emoji /g'
cpp.json: 🔒
global.json.code-snippets: 👻
markdown.json: 🔒
rust.json: 🔒
=================================================================================================================================================================================================
git diff --stat .
=================================================================================================================================================================================================
 .config/Code/User/snippets/global.json.code-snippets | 72 ++++++++++++++++++++++++++++++++++++------------------------------------
 1 file changed, 36 insertions(+), 36 deletions(-)
```

## how to install
``` bash
install_path="$HOME/local/bin/"
wgit https://raw.githubusercontent.com/umaumax/git-sed/master/git-sed -O "$install_path/git-sed"
wgit https://raw.githubusercontent.com/umaumax/git-sed/master/git-fixedsed -O "$install_path/git-fixedsed"
chmod u+x "$install_path/git-sed"
chmod u+x "$install_path/git-fixedsed"
```
