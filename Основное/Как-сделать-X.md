# Как сделать X

**Русификация игры**

+ Скачать архив с русификатором из общей папки [mega:share](https://link.meridiano-web.com/mega:share)/Starfield, файл "Starfield-Russian-2.4.1.zip".
+ Проверить, чтобы не было установлено других переводов.
+ Папку Data совместить с папкой Data в корне игры, содержимое StarfieldCustom.ini совместить с содержимым файла по пути "Документы/My Games/Starfield/StarfieldCustom.ini".

**Убрать Message Of The Day**

+ Откройте файл "Документы/My Games/Starfield/StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bEnableMessageOfTheDay=0" без кавычек.

**Более приятный интерфейс**

+ Используйте [Undelayed Menus](https://www.nexusmods.com/starfield/mods/404) для быстрых переходов и 60 FPS.
+ Для компактного интерфейса - [моды Stentorious](https://www.nexusmods.com/starfield/users/13373850?tab=user+files) из серии Compact UI.
+ Не забудьте про патчи совместимости между всеми модами.

**Убрать фон субтитров**

+ Используйте [Spicy Clean Subtitles](https://www.nexusmods.com/starfield/mods/539) (с патчами по необходимости).

**Заменить изображение при запуске**

+ По пути "Config/Images" в корне игры находится файл "SplashScreen1920x1080.png".
+ Можете заменить его на любое изображение, даже с прозрачностью.

**Пропустить интро и прочие мелочи**

+ Отключить видео BGS: по пути "Data/Video" в корне игры переименовать файл "BGS_LOGO_1080p_BinkVersion.bk2" в "BGS_LOGO_1080p_BinkVersion.bk2.backup".
+ Отключить интро, ускорить переходы: правьте "Документы/My Games/Starfield/StarfieldCustom.ini".
```
[Camera]
iDialogueTransitionMillis=10

[General]
fAutoDoorFadeSecs=0.0001
fFastTravelFadeSecs=0.0001
fLoadGameFadeSecs=0.0001
fNormalDoorFadeSecs=0.0001
fNormalDoorFadeWait=0.0001

[Dialogue]
bDialogueDelayMenuExit=0.001
sIntroSequence=0
uMainMenuDelayBeforeAllowSkip=0

[Interface]
fFadeToBlackFadeSeconds=0.0001
fSleepFaderTime=0.0001
fDataMenuFadeInToGameTime=0.0001
```

**Джетпак через удержание клавиши**

+ Откройте файл "Документы/My Games/Starfield/StarfieldCustom.ini".
+ В секции [Boostpack] добавьте параметр "bUsePressAndHoldControls=1" без кавычек.

**Изменить цветофильтр (по возможности)**

+ Чтобы отключить, используйте [Neutral LUTs - No Color Filters](https://www.nexusmods.com/starfield/mods/323). Прочитайте описание, там есть и ini-твики.
+ Чтобы просто ослабить, используйте [Reduced LUTs - Cleaner Colors and Enhanced Contrast](https://www.nexusmods.com/starfield/mods/589).

**Настройка входящего/исходящего урона**

+ Содержится в [Gameplay Tweaks and Fixes](https://www.nexusmods.com/starfield/mods/241). Мод представляет из себя bat-файл, который применяется при загрузке и меняет настройки.

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
+ В секции [Dialogue] добавьте параметры "fDialogueCameraCollisionRadius=2.0" и "fDialogueCameraFailsafeFPFOV=100.0". Это опционально, для отключения приближения камеры в диалогах.

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