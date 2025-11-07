#### How to use

WSL上で実施

```shell
git clone --recursive https://github.com/norikmb/AutoZA.git
sudo apt install gcc-avr avr-libc avrdude make
```

lufa/LUFA/Drivers/Board/Buttons.h の98行目を以下のように変更

```c
        static inline uint8_t    Buttons_GetStatus(void) { return 0; }
```

コンパイルする

```shell
make
```
