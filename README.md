# git-sed

## how to use
```
git-sed 's/double/float/g' ':*.cpp'
git-fixedsed '/root' '/user/hoge' ':*.cpp'
```

## how to install
```
install_path="$HOME/local/bin/"
wgit https://raw.githubusercontent.com/umaumax/git-sed/master/git-sed -O "$install_path/git-sed"
wgit https://raw.githubusercontent.com/umaumax/git-sed/master/git-fixedsed -O "$install_path/git-fixedsed"
chmod u+x "$install_path/git-sed"
chmod u+x "$install_path/git-fixedsed"
```
