# Как сделать X

> Внимание! Если мод требует правок в ini-файлах StarfieldCustom.ini или SkyrimPrefs.ini, то вы должны точно знать, откуда эти файлы будут читаться игрой. Если вы не используете MO2 или в вашем профиле MO2 отключена опция "profile-specific ini files", то ini-файлы читаются из папки "Документы/My Games/Starfield". В остальных случаях они читаются из папки вашего профиля MO2. Будьте внимательны к этому при внесении изменений.

**Русификация игры**

+ Скачать архив с русификатором из общей папки [mega:share](https://link.meridiano-web.com/mega:share)/Starfield, файл "Starfield-Russian-2.5.1.zip".
+ Проверить, чтобы не было установлено других переводов.
+ Установить архив как мод в MO2, внести правки StarfieldCustom.ini в вашу версию этого файла.

**Убрать Message Of The Day**

+ Правка файла "StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bEnableMessageOfTheDay=0" без кавычек.

**Более приятный интерфейс**

+ Используйте [Undelayed Menus](https://www.nexusmods.com/starfield/mods/404) для быстрых переходов и 60 FPS.
+ Для компактного интерфейса - [моды Stentorious](https://www.nexusmods.com/starfield/users/13373850?tab=user+files) из серии Compact UI.
+ Для подробного интерфейса - [StarUI Inventory](https://www.nexusmods.com/starfield/mods/773).
+ Учитывайте порядок перезаписи в MO2, файлы одних модов перезаписывают другие.

**Убрать фон субтитров**

+ Используйте [Spicy Clean Subtitles](https://www.nexusmods.com/starfield/mods/539) (с патчами по необходимости).

**Заменить изображение при запуске**

+ По пути "Config/Images" в корне игры находится файл "SplashScreen1920x1080.png".
+ Можете заменить его на любое изображение, даже с прозрачностью.

**Пропустить интро и прочие мелочи**

+ Отключить видео BGS: по пути "Data/Video" в корне игры переименовать файл "BGS_LOGO_1080p_BinkVersion.bk2" в "BGS_LOGO_1080p_BinkVersion.bk2.backup".
+ Отключить интро, ускорить переходы: правки файла "StarfieldCustom.ini".
```
[Camera]
iDialogueTransitionMillis=10

[General]
fAutoDoorFadeSecs=0.001
fFastTravelFadeSecs=0.001
fLoadGameFadeSecs=0.001
fNormalDoorFadeSecs=0.001
fNormalDoorFadeWait=0.001

[Dialogue]
bDialogueDelayMenuExit=0.001
uMainMenuDelayBeforeAllowSkip=0

[Interface]
fSleepFaderTime=0.001
fFadeToBlackFadeSeconds=0.001
fDataMenuFadeInToGameTime=0.001
```

**Джетпак через удержание клавиши**

+ Правка файла "StarfieldCustom.ini".
+ В секции [Boostpack] добавьте параметр "bUsePressAndHoldControls=1" без кавычек.

**Изменить цветофильтр (по возможности)**

+ Чтобы отключить, используйте [Neutral LUTs - No Color Filters](https://www.nexusmods.com/starfield/mods/323). Прочитайте описание, там есть и ini-твики.
+ Чтобы просто ослабить, используйте [Reduced LUTs - Cleaner Colors and Enhanced Contrast](https://www.nexusmods.com/starfield/mods/589).

**Настройка входящего/исходящего урона**

+ Содержится в [Gameplay Tweaks and Fixes](https://www.nexusmods.com/starfield/mods/241). Мод представляет из себя bat-файл, который применяется при загрузке и меняет настройки.

**Убивать бессмертных NPC** (не рекомендуется)

+ Правка файла "StarfieldCustom.ini".
+ В секции [GamePlay] добавьте параметр "bEssentialTakeNoDamage=0" без кавычек.

**Отключить паузу у свёрнутой игры**

+ Правка файла "StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bAlwaysActive=1" без кавычек.

**Настроить FOV камеры**

+ Правки файла "StarfieldCustom.ini".
+ В секции [Camera] добавьте параметры "fFPWorldFOV=100.0", "fTPWorldFOV=100.0" и "fDefaultFOV=100.0" без кавычек.
+ В секции [FlightCamera] добавьте параметр "fFlightCameraFOV=100.0" без кавычек.
+ В секции [Dialogue] добавьте параметры "fDialogueCameraCollisionRadius=2.0" и "fDialogueCameraFailsafeFPFOV=100.0". Это опционально, для отключения приближения камеры в диалогах.

**Отключить границы при исследовании планеты**

+ Правка файла "StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bBorderRegionsEnabled=0" без кавычек.
+ Внимание! При заходе слишком далеко игра становится нестабильной и крашится.

**Включить достижения Steam обратно**

+ Используйте [Baka Achievement Enabler](https://www.nexusmods.com/starfield/mods/658), установите его как обычный мод в MO2.
+ Требуется SFSE, инструкция по установке есть в [Установке модов](../Моддинг/Установка-модов.md).

------

|[*Назад к оглавлению*](https://github.com/Meridiano/Starfield-Head)|
|:---:|