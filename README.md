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

## Sources

* [Хеш-стеганография в dataset-ах. На этот раз быстрая](https://www.pvsm.ru/python/276026)
* [ECB mode](https://pycryptodome.readthedocs.io/en/latest/src/cipher/classic.html#ecb-mode)
* [Семантическая стойкость](https://ru.wikipedia.org/wiki/%D0%A1%D0%B5%D0%BC%D0%B0%D0%BD%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B0%D1%8F_%D1%81%D1%82%D0%BE%D0%B9%D0%BA%D0%BE%D1%81%D1%82%D1%8C)
