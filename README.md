# Route 365 or Codeforces Test tool (Linux, MacOS)

Original script [GitHub kirumbik pages](https://gist.github.com/kirumbik/48a2b404cfbcd35b3aba9acbc56ba226)

##Usage
Let's pretend you have directory contest where you store contest code. Place run_tests.sh script in root of contest directory.
Place tests near you go code:
```
./b/main.go
./b/tests/
|----01
|----01.a
|----...
|----08
|----08.a
./c/main.go
./c/tests/
|----01
|----01.a
|----...
```


After that run:
```./run_tests.sh ./b/main.go```

You will see each test running:
![src_img2](https://gist.github.com/assets/11439553/7216b60c-cc29-45be-a640-f57b85a53bb3)

###MacOS info

- install homebrew
- brew install dos2unix
- brew install diffutils
- brew install coreutils
- add gnubin into your PATH variable
```PATH="/usr/local/opt/coreutils/libexec/gnubin:$PATH"```
or check
```export PATH="/opt/homebrew/opt/coreutils/libexec/gnubin:$PATH"``` in ```.zshrc```

if u have time problem use:
```export LC_NUMERIC="en_US.UTF-8"```
