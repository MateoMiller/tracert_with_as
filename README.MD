Таск по "Протоколы Интернет"
Исполнил Гусев Юрий КН-203

Справка по использованию:
Запуск через консоль:
py main.py Куда_хотим_обратиться.net

Примеры использования
Пример1)
    input:
    py main.py 8.8.8.8
    
    output:
    №    Ip              AS              Country   Provider
    1    192.168.0.1     None            None      None
    2    10.0.139.1      None            None      None
    3    172.30.5.8      None            None      None
    4    188.254.26.108  AS12389         RU        ROSTELECOM-MNT
    5    188.254.25.115  AS12389         RU        ROSTELECOM-MNT
    6    87.226.215.130  AS12389         RU        ROSTELECOM-MNT
    7    87.251.181.53   AS5563          RU        AS5563-MNT
    8    82.193.138.167  AS5563          RU        RIPE-NCC-HM-MNT
    9    10.255.100.1    None            None      None
    10   10.255.15.1     None            None      None
    
Пример:
    input:
    py main.py urfu.ru
    
    output:
    №    Ip              AS              Country   Provider
    1    192.168.0.1     None            None      None
    2    10.0.139.1      None            None      None
    3    172.30.5.8      None            None      None
    4    188.254.26.108  AS12389         RU        ROSTELECOM-MNT
    5    188.254.25.115  AS12389         RU        ROSTELECOM-MNT
    6    87.226.215.130  AS12389         RU        ROSTELECOM-MNT
    7    87.251.181.53   AS5563          RU        AS5563-MNT
    8    82.193.138.167  AS5563          RU        RIPE-NCC-HM-MNT
    9    10.255.100.1    None            None      None
    10   10.255.15.1     None            None      None
    
Дополнительно:
    В коде есть неочевидная обработка ошибок.
    Если отсутствует интернет, проблемы с DNS или ещё что-то, то консольная утилита tracert не вернет ip адреса,
    и мы не будем обращаться к nic.ru.
    Если проблемы в обращении к nic.ru, то этот кейс обработан
