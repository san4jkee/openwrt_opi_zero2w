# Build OpenWRT for Orange Pi Zero 2w

<h3>Записать образ с помощью программы Raspberry Pi Imager</h3>
<ul>
<li>
После записи переподключить карту и в файле Env.txt заменить sun50i-h618-orangepi-zero2w.dtb на sun50i-h616-orangepi-zero2w.dtb <br>
Изменить overlay_prefix=sun50i-h618 на overlay_prefix=sun50i-h616
</li>
<li>
В директории extlinux в конфиг файле extlinux.conf так же заменить на sun50i-h616-orangepi-zero2w.dtb
</li>
<li>Вставляем флешку  плату и запускем. После запуска появится точка доступа A2 без пароля. Подключаемся к ней и заходим по ссылке http://192.168.1.1/</li>
</ul>

