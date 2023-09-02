# Как сделать X

**Русификация интерфейса**

+ Скачать архив с русификатором из общей папки [mega:share](https://link.meridiano-web.com/mega:share)/Starfield, файл "Starfield-Rus-0.1.7z".
+ Внести содержимое ini-файла архива в ini-файл игры по адресу "Документы/My Games/Starfield/StarfieldCustom.ini", если файла нет - просто скопируйте его.
+ Скопировать содержимое папки Data архива в папку Data игры.

**Русификация всего**

+ Скачать архив с русификатором из общей папки [mega:share](https://link.meridiano-web.com/mega:share)/Starfield, файл "DeepL-Dialogs-Alpha.zip".
+ 01-Shared: обязательно для установки. Папку Data совместить с папкой Data в корне игры, содержимое StarfieldCustom.ini совместить с содержимым StarfieldCustom.ini в Документах.
+ 02-DeepL-Dialogs или 03-Alpha-Version: на выбор одно из двух. Первое только диалоги, второе - альфа-версия всего. Папку Data совместить с папкой Data в корне игры.

**Убрать Message Of The Day**

+ Откройте файл "Документы/My Games/Starfield/StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bEnableMessageOfTheDay=0" без кавычек.

**Заменить изображение при запуске**

+ По пути "Config/Images" в корне игры находится файл "SplashScreen1920x1080.png".
+ Можете заменить его на любое изображение, даже с прозрачностью.

**Отключить видео Bethesda Game Studios**

+ По пути "Data/Video" в корне игры переименовать файл "BGS_LOGO_1080p_BinkVersion.bk2" в "BGS_LOGO_1080p_BinkVersion.bk2.backup".

**Убивать бессмертных NPC** (не рекомендуется)

+ Откройте файл "Документы/My Games/Starfield/StarfieldCustom.ini".
+ В секции [GamePlay] добавьте параметр "bEssentialTakeNoDamage=0" без кавычек.

**Отключить паузу у свёрнутой игры**

+ Откройте файл "Документы/My Games/Starfield/StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bAlwaysActive=1" без кавычек.

**Настроить FOV камеры**

+ Откройте файл "Документы/My Games/Starfield/StarfieldCustom.ini".
+ В секции [Camera] добавьте параметры "fFPWorldFOV=100.0", "fTPWorldFOV=100.0" и "fDefaultFOV=100.0" без кавычек.
+ В секции [FlightCamera] добавьте параметр "fFlightCameraFOV=100.0" без кавычек.

**Отключить границы при исследовании планеты**

+ Откройте файл "Документы/My Games/Starfield/StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bBorderRegionsEnabled=0" без кавычек.
+ Внимание! При заходе слишком далеко игра становится нестабильной и крашится.

**Включить достижения Steam обратно**

+ Используйте [Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader/releases/latest) и [Achievement Enabler](https://www.nexusmods.com/starfield/mods/252).
+ Внимательно следуйте инструкции по установке на странице Achievement Enabler!

------

|[*Назад к оглавлению*](https://github.com/Meridiano/Starfield-Head)|
|:---:|