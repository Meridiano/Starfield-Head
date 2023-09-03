# Как сделать X

**Русификация игры**

+ Скачать архив с русификатором из общей папки [mega:share](https://link.meridiano-web.com/mega:share)/Starfield, файл "Starfield-Russian-2.4.1.zip".
+ Проверить, чтобы не было установлено других переводов.
+ Папку Data совместить с папкой Data в корне игры, содержимое StarfieldCustom.ini совместить с содержимым файла по пути "Документы/My Games/Starfield/StarfieldCustom.ini".

**Убрать Message Of The Day**

+ Откройте файл "Документы/My Games/Starfield/StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bEnableMessageOfTheDay=0" без кавычек.

**Заменить изображение при запуске**

+ По пути "Config/Images" в корне игры находится файл "SplashScreen1920x1080.png".
+ Можете заменить его на любое изображение, даже с прозрачностью.

**Отключить видео Bethesda Game Studios**

+ По пути "Data/Video" в корне игры переименовать файл "BGS_LOGO_1080p_BinkVersion.bk2" в "BGS_LOGO_1080p_BinkVersion.bk2.backup".

**Убрать цветофильтр (по возможности)**

+ Используйте [Neutral LUTs - No Color Filters](https://www.nexusmods.com/starfield/mods/323). Прочитайте описание, там есть и ini-твики.

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