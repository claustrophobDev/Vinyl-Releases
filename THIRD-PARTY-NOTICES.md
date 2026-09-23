# Компоненты других авторов

Vinyl распространяется вместе с чужим софтом. Он остаётся под своими лицензиями,
лицензия Vinyl на него не распространяется. Тексты лицензий лежат в папке `licenses`
рядом с программой.

## sing-box

Ядро, которое поднимает туннель. Запускается отдельным процессом, Vinyl общается с ним
через конфиг и локальный api.

- Автор: nekohasekai и участники проекта
- Лицензия: GNU General Public License v3.0 или новее
- Исходный код: https://github.com/SagerNet/sing-box
- В сборке: `core\sing-box.exe`, текст лицензии — `licenses\sing-box-LICENSE.txt`

## Wintun

Драйвер сетевого адаптера, через него работает туннельный режим. Используется ядром
sing-box через публичный API wintun.h.

- Автор: WireGuard LLC
- Лицензия: Prebuilt Binaries License (распространение готовой dll разрешено, если она
  идёт вместе с софтом, который использует её только через заявленный API)
- Сайт: https://www.wintun.net
- В сборке: `core\wintun.dll`, текст лицензии — `licenses\wintun-LICENSE.txt`

## nlohmann/json

Заголовочная библиотека для JSON, собирается внутрь `vinyl.exe`.

- Автор: Niels Lohmann
- Лицензия: MIT
- Исходный код: https://github.com/nlohmann/json
- Текст лицензии — `licenses\nlohmann-json-LICENSE.txt`

## Списки маршрутов

Наборы правил для рф-сайтов и подсетей, скачиваются при сборке и обновляются программой.

- Источник: https://github.com/SagerNet/sing-geosite и https://github.com/SagerNet/sing-geoip
- В сборке: `geo\*.srs`
