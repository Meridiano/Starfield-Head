# Как сделать X

> Внимание! Если мод требует правок в ini-файлах StarfieldCustom.ini или SkyrimPrefs.ini, то вы должны точно знать, откуда эти файлы будут читаться игрой. Если вы не используете MO2 или в вашем профиле MO2 отключена опция "profile-specific ini-files", то ini-файлы читаются из папки "Документы/My Games/Starfield". В остальных случаях они читаются из папки вашего профиля MO2. В любом из двух случаев вы можете использовать редактор ini-файлов игры, встроенный в MO2, он всегда открывает именно те файлы, которые читаются игрой.

**Русификация игры**

+ Скачать архив с русификатором из общей папки [mega:share](https://link.meridiano-web.com/mega:share)/Starfield, файл "Starfield-Russian-0.4.2.zip".
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

**Выбор опций диалога по цифрам**

+ Используйте [Better Dialogue Controls](https://www.nexusmods.com/starfield/mods/1223).

**Заменить изображение при запуске**

+ По пути "Config/Images" в корне игры находится файл "SplashScreen1920x1080.png".
+ Можете заменить его на любое изображение, даже с прозрачностью.

**Пропустить интро и прочие мелочи**

+ Правки файла "StarfieldCustom.ini".
```
[Camera]
iDialogueTransitionMillis=10

[General]
fAutoDoorFadeSecs=0.001
fFastTravelFadeSecs=0.001
fLoadGameFadeSecs=0.001
fNormalDoorFadeSecs=0.001
fNormalDoorFadeWait=0.001
sIntroSequence=?
uMainMenuDelayBeforeAllowSkip=0

[Dialogue]
bDialogueDelayMenuExit=0.001

[Interface]
fSleepFaderTime=0.001
fFadeToBlackFadeSeconds=0.001
fDataMenuFadeInToGameTime=0.001
```

**Джетпак через удержание клавиши**

+ Правка файла "StarfieldCustom.ini".
+ В секции [Boostpack] добавьте параметр "bUsePressAndHoldControls=1" без кавычек.

**Изменить цветофильтр (по возможности)**

+ Чтобы отключить, используйте [Neutral LUTs - No Color Filters](https://www.nexusmods.com/starfield/mods/323).
+ Чтобы просто ослабить, используйте [Reduced LUTs - Cleaner Colors and Enhanced Contrast](https://www.nexusmods.com/starfield/mods/589).

**Более чёрный космос**

+ Правки файла "StarfieldCustom.ini".
```
[Display]
fSpaceGlowBackgroundScale=0.0
fStarIntensity=2500.0
fStarSystemFarViewDistance=10000000000.0
fStarfieldBackgroundScale=35.0
fStarfieldStarBrightnessScale=10.0
fStarfieldStarCoordScale=10.0
fSunScale=1.0
```

**Убрать "ультразвук" из меню**

+ Используйте [Starfield High Pitch SFX Tinnitus Fix](https://www.nexusmods.com/starfield/mods/787).

**Уменьшение времени сканирования до 1 сек.**

+ Используйте [Instant Scan](https://www.nexusmods.com/starfield/mods/759). Мод представляет из себя bat-файл, который вы должны применять при загрузке. Прочтите инструкцию по установке.

**Настройка урона и кол-ва здоровья врагов**

+ Содержится в [Gameplay Tweaks and Fixes](https://www.nexusmods.com/starfield/mods/241). Мод представляет из себя bat-файл, который применяется при загрузке и меняет настройки.

**Быстрые переходы у верстаков и т.д.**

+ [Faster Workbenches](https://www.nexusmods.com/starfield/mods/1190).
+ [Faster Pilot Seats](https://www.nexusmods.com/starfield/mods/1237).
+ [Faster switch from combat to relaxed stance](https://www.nexusmods.com/starfield/mods/1148).
+ [Ship Skip - Instant Station Docking and More](https://www.nexusmods.com/starfield/mods/1056).

**Изменить гамму (2.4 по умолчанию)**

+ Правка файла "StarfieldCustom.ini".
+ В секции [Display] добавьте параметр "fGamma=2.6" без кавычек.

**Качественные текстуры эффектов**

+ Используйте [Effect Textures Enhanced](https://www.nexusmods.com/starfield/mods/340).

**Убивать бессмертных NPC** (не рекомендуется)

+ Правка файла "StarfieldCustom.ini".
+ В секции [GamePlay] добавьте параметр "bEssentialTakeNoDamage=0" без кавычек.

**Отключить паузу у свёрнутой игры**

+ Правка файла "StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bAlwaysActive=1" без кавычек.

**Настроить FOV камеры**

+ Правки файла "StarfieldCustom.ini".
```
[Camera]
fFPWorldFOV=100.0
fTPWorldFOV=100.0
fDefaultFOV=100.0

[FlightCamera]
fFlightCameraFOV=100.0

[Dialogue]
fDialogueCameraCollisionRadius=2.0
fDialogueCameraFailsafeFPFOV=100.0
```

**Быстрое перетаскивание предметов**

+ Правки файла "StarfieldCustom.ini".
```
[Controls]
fQCZKeyDelay=0.05
fZKeyDelay=0.05
```

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