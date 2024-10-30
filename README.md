# Build OpenWRT for Orange Pi Zero 2w

<h3>Записать образ с помощью программы Raspberry Pi Imager</h3>
<a href="https://drive.google.com/file/d/17hGM75TAPYJdETZpkkIjkqb-2UBARsHy/view?usp=sharing" target="_blank">Ссылка на образ</a>
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

<h3>Для входного подключения я использую WIFI USB-адаптер Mediatek MT7601u</h3>
<p>Для его работы нужно установить драйвера, находятся в директории package</p>

<p>Для их установки заходим в <b>System -> Software</b>, нажимаем кнопку Upload Package и сперва загружаем mt7601u-firmware_20230804-1_aarch64_generic. После успешной загрузки загружаем kmod-mt7601u_5.15.162+6.1.97-1-1_aarch64_generic</p>
<p>После этого в списке беспроводных сетей появится новое устройство Generic MAC80211 802.11b/g/n</p>
