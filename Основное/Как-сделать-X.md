# Как сделать X

> Внимание! Если мод требует правок в ini-файлах StarfieldCustom.ini или SkyrimPrefs.ini, то вы должны точно знать, откуда эти файлы будут читаться игрой. Если вы не используете MO2 или в вашем профиле MO2 отключена опция "profile-specific ini-files", то ini-файлы читаются из папки "Документы/My Games/Starfield". В остальных случаях они читаются из папки вашего профиля MO2. В любом из двух случаев вы можете использовать редактор ini-файлов игры, встроенный в MO2, он всегда открывает именно те файлы, которые читаются игрой.

## Интерфейс

**Русификация игры**

+ Скачать архив с русификатором из общей папки [mega:share](https://link.meridiano-web.com/mega:share)/Starfield, файл "Starfield-Russian-0.4.2.zip".
+ Проверить, чтобы не было установлено других переводов.
+ Установить архив как мод в MO2, внести правки StarfieldCustom.ini в вашу версию этого файла.

**Убрать Message Of The Day**

+ Правка файла "StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bEnableMessageOfTheDay=0" без кавычек.

**Более приятный интерфейс**

+ В качестве основы используйте Smooth UI, [60 FPS](https://www.nexusmods.com/starfield/mods/350) или [120 FPS](https://www.nexusmods.com/starfield/mods/497).
+ Используйте [Undelayed Menus](https://www.nexusmods.com/starfield/mods/404) для быстрых переходов.
+ Для компактного интерфейса - [моды Stentorious](https://www.nexusmods.com/starfield/users/13373850?tab=user+files) из серии Compact UI.
+ Для подробного интерфейса - [StarUI Inventory](https://www.nexusmods.com/starfield/mods/773).
+ Учитывайте порядок перезаписи модов и патчей в MO2, файлы одних перезаписывают другие.

**Убрать фон субтитров**

+ Используйте [Spicy Clean Subtitles](https://www.nexusmods.com/starfield/mods/539) (с патчами по необходимости).

**Выбор опций диалога по цифрам**

+ Используйте [Better Dialogue Controls](https://www.nexusmods.com/starfield/mods/1223).

**Убрать "ультразвук" из меню**

+ Используйте [Starfield High Pitch SFX Tinnitus Fix](https://www.nexusmods.com/starfield/mods/787).

## Функционал

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
; установка FOV в диалогах
fDialogueCameraCollisionRadius=2.0
fDialogueCameraFailsafeFPFOV=100.0
```

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

**Быстрое перетаскивание предметов**

+ Правки файла "StarfieldCustom.ini".
```
[Controls]
fQCZKeyDelay=0.05
fZKeyDelay=0.05
```

**Джетпак через удержание клавиши**

+ Правка файла "StarfieldCustom.ini".
+ В секции [Boostpack] добавьте параметр "bUsePressAndHoldControls=1" без кавычек.

**Уменьшение времени сканирования до 1 сек.**

+ Используйте [Instant Scan](https://www.nexusmods.com/starfield/mods/759).
+ Мод представляет из себя bat-файл, который вы должны применять при загрузке. Прочтите инструкцию по установке.

**Настройка урона и кол-ва здоровья врагов**

+ Содержится в [Gameplay Tweaks and Fixes](https://www.nexusmods.com/starfield/mods/241).
+ Мод представляет из себя bat-файл, который вы должны применять при загрузке. Прочтите инструкцию по установке.

**Быстрые переходы у верстаков и т.д.**

+ [Faster Workbenches](https://www.nexusmods.com/starfield/mods/1190).
+ [Faster Pilot Seats](https://www.nexusmods.com/starfield/mods/1237).
+ [Faster switch from combat to relaxed stance](https://www.nexusmods.com/starfield/mods/1148).
+ [Ship Skip - Instant Station Docking and More](https://www.nexusmods.com/starfield/mods/1056).

## Графика

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

**Изменить гамму** (2.4 по умолчанию)

+ Правка файла "StarfieldCustom.ini".
+ В секции [Display] добавьте параметр "fGamma=2.6" без кавычек.

**Качественные текстуры эффектов**

+ Используйте [Effect Textures Enhanced](https://www.nexusmods.com/starfield/mods/340).

**Заменить изображение при запуске**

+ По пути "Config/Images" в корне игры находится файл "SplashScreen1920x1080.png".
+ Можете заменить его на любое изображение, даже с прозрачностью.

## Прочее

**Добавить трейты на броню**

+ Выбросьте предмет на землю и выберите его в консоли (должен быть тип ARMO, ID FFXXXXXX).
+ Используйте консольную команду AMod, чтобы изменить базовое качество брони.
```
﻿11E2BB    mod_Armor_Spacesuit_Quality_01
11E2BC    mod_Armor_Spacesuit_Quality_02
11E2BA    mod_Armor_Spacesuit_Quality_03
11E2B9    mod_Armor_Spacesuit_Quality_04
03AF7D    mod_Armor_Spacesuit_Quality_05
```
+ Эта же команда может добавлять броне трейты, максимум 3 трейта, по одному из каждой группы.
```
Группа #1

sensor chip       2c43db    ﻿+20% acc while moving
sentinel          0be540﻿    75% chance to take 50% less dmg while not moving
headhunter        2c43dc﻿    +25% dmg on next attack after a headshot
armor plated      2ede59﻿    -10% dmg from physical,energy and em
mechanized        0be542﻿    +40 carry capacity
assisted carry    2EDE4F﻿    reduces o2 consumption while encumbered by 75%
incendiary        002983﻿    10% chance to ignite nearby attackers
mirrored          059ae8﻿    4% chance to reflect attacks
repulsing         06029d﻿    5% chance to disarm nearby attackers

Группа #2

o2 boosted        0690b0﻿    +20% oxygen
combat veteran    1336be﻿    -15% dmg from humans
beast hunter      1336bd﻿-    15% dmg from aliens
chameleon         1336c1﻿    makes you invisible in sneak while not moving
ablative          13369c﻿    -15% incoming energy damage
incendiary        002983﻿    10% chance to ignite nearby attackers
sturdy            133699﻿    -15% incoming melee dmg
o2 filter         0690ae﻿    -25% oxygen consumption
bolstering        1336c6﻿    grants up to +100 energy and physical resistance, the lower your health
technician        1336bc﻿    -15% dmg from robots
anti-ballistic    13369e﻿    -15% incoming dmg from ranged weapons

Группа #3

fastened           2ede4e﻿    +20 carry capacity
auto medic         0c9a43﻿    automatically use a med pack when hit and health is below 25%, 60s cd
galvanized         0710f7﻿    +25 corrosive resistance
incendiary         07d728﻿    randomly deal fire damage (works with the other incendiary mod too)
liquid cooled      0710f6﻿    +25 thermal resistance
resource hauler    060293﻿    resources weigh 25% less
analyzer           0690af﻿    +10% dmg to scanned targets
leadlined          0710f5﻿    +25 radiation resistance
hacker             2c43da﻿    +2 max auto attempts that can be banked while hacking
weapon holsters    060295    weapons weigh 50% less
acrobat            0710fd﻿    reduces fall dmg by 50%
antiseptic         0710fa﻿    +25 airborne resistance
staggering         0e8d64﻿    small chance to stagger enemies
```

**Убивать бессмертных NPC** (не рекомендуется)

+ Правка файла "StarfieldCustom.ini".
+ В секции [GamePlay] добавьте параметр "bEssentialTakeNoDamage=0" без кавычек.

**Отключить паузу у свёрнутой игры**

+ Правка файла "StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bAlwaysActive=1" без кавычек.

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