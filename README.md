# linux_xorg_glamor_perfomance_uxa_tearing_obs_studio_fix_intel
linux_xorg_glamor_perfomance_uxa_intel_double_SPEED2X

!Danger! black screen repair boot recovery console and tty ALT-SHIFT-F2 and F3 , F4 , F5 , F6 ,F8 login command ↓↓↓

$ sudo rm - rf /etc/X11/xorg.conf

$ sudo rm - rf /etc/X11/xorg.conf.failsafe

$ sudo rm - rf /usr/share/X11/xorg.conf.d/20-nouveau.conf

$ sudo rm - rf /usr/share/X11/xorg.conf.d/20-intel.conf

$ sudo rm - rf /etc/X11/xorg.conf.d

$ sudo service lightdm restart 

and gdm , gdm3 manager-session ? ОK ↓↓↓ 

$ sudo service gdm restart

$ sudo service gdm3 restart 

Not systemd ? Not problem session restart. Ок example ↓↓↓ 

$ sudo /usr/sbin/lightdm restart

$ sudo systemctl /usr/sbin/lightdm restart

gnome manager-session ?

$ sudo /usr/sbin/gdm restart

and not job command ? ok variant 2 command ↓↓↓

$ sudo systemctl /usr/sbin/gdm restart

gnome 3 manager-session ? 

$ sudo /usr/sbin/gdm3 restart

and not job command ? ok variant 2 command ↓↓↓

$ sudo systemctl /usr/sbin/gdm3 restart

__________________________________________________________________________________________________________________________

run terminal in folder script command:

$ chmod +x Install_xorg_intel_perfomance_yes.sh and / или Install_xorg_fbdev_accel_method_glamor_perfomance_yes.sh

run in terminal запустите как в терминале , а можете перетащить фаил Install_xorg_intel_perfomance_yes.sh на любой терминал и нажать ENTER затребует пароль в состав входит даже деинсталятор он появится когда скрипт будет исполнен или самим сделать исполняемым и запустить в терминале потребует пароль и установит после надо будет перезагрузить компьютер.

Xorg nvidia alternative nouveau xorg_nouveau_accel_method_glamor_perfomance выполнить этот скрипт в онлайне для установки драивера.

Проверить как загрузился драивер

$ inxi -G

Осталось отремонтировать эти два фаила i965_dri.so и i915_dri.so   /usr/lib/x86_64-linux-gnu/dri дело в том что именно эти 
драивера хорга вроде все быстро и нету qemu тиринга , но есть одно но когда obs-studio на весь экран то видны именно эти дигональные черные тиринговые мерцания и дикое смещение за отступы в нем на другую сторону т.е если вы подмените с другого дистра фаилы и что самое важное сделаете соответствующие права то вы тоже по идее получите высокую скорость , но будет что то типа qemu без гпу ускорения и возможности переключать клавиатуру в играх , но будет зато переключаться язык если вы деконфигурируете клавиатуру из консоли и выставите там alt+shift то он и работать будет даже там где ранее можно было переключать по другому типа super+space или super+shift так как и она видимо очень завязана с этим фаилом. Как бы без псевдо научных теории я рассказал на опыте почему там именно такой тиринг в obs-studio. 
Как пример dri_от_void но внимание опасно т.е я не знаю заведетс у вас или нет я делал это на своем созданном дистрибутиве 19.04 и только что бы это был синнамон 2D сам другой dri https://dropmefiles.com.ua/zMwZ2 потом проверяем открываем obs-studio , а можно просто взять эти два фаила i965_dri.so и i915_dri.so и подменить их и внимание не обходимо выставлять права! Что бы потом не поимать экран это уже сами ищите кому надо наидут. Делаем так же замер производительности в программе hadrinfo но только с условием что все so заменены из архива тогда производительность будет самая высокая.

Взяли и распространяете ссылка на оригинал обязательна.

Не обещается исправление тиринга во всех программах , но в obs уже такого дикого тиринга нет небольшая диагональ зато производительность glamor в два раза выше , в случае чего если вам вообще не нужен тиринг то есть оптимальная производительность , но только будет ровно пол скорости конфиг ниже.
_______________________________________________________________________________________________________________________________

Я бы поискал такие же готовые решения для амд , нвидиа и других , но это надо денег на оборудование потому что вулкан это профанация и деньги ушли туда на какой то костыль в который поверили оно и так понятно было опенжл так что просто пробуйте в скриптах поменять intel на свою карту







