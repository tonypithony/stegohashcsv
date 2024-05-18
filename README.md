# CHS
Csv Hash Steganography

Хеш стеганография, реализованная в CSV данных

См. пост: https://habrahabr.ru/post/339432/


## Команды
Сгенерировать CSV файл с сообщением:
```bash
$ python chs.py -m "text message" -i world-cities.csv -o stego.csv  
$ Введите пароль: 123456789123456789
```

Извлечь сообщение:
```bash
$ python3 chs.py -i stego.csv  
$ Введите пароль: 123456789123456789  
$ Извлечённое сообщение:'text message'  
```


Красивая гифка как это работает:

![](https://habrastorage.org/webt/qa/ly/is/qalyisqcgndlts0dgbkykmfg2fa.gif)


## Зависимости

```bash
$ pip install pycryptodome mmh3
```

![](https://raw.githubusercontent.com/tonypithony/stegohashcsv/master/data/test-stegohash.PNG)
