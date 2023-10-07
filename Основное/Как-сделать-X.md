# Как сделать X

> Внимание! Если мод требует правок в ini-файлах StarfieldCustom.ini или SkyrimPrefs.ini, то вы должны точно знать, откуда эти файлы будут читаться игрой. Если вы не используете MO2 или в вашем профиле MO2 отключена опция "profile-specific ini-files", то ini-файлы читаются из папки "Документы/My Games/Starfield". В остальных случаях они читаются из папки вашего профиля MO2. В любом из двух случаев вы можете использовать редактор ini-файлов игры, встроенный в MO2, он всегда открывает именно те файлы, которые читаются игрой.

## Интерфейс

**Русификация игры**

+ Скачать архив с русификатором из общей папки [mega:share](https://link.meridiano-web.com/mega:share)/Starfield, файлы "Starfield-Russian" на выбор.
+ Проверить, чтобы не было установлено других переводов.
+ Установить архив как мод в MO2, внести правки StarfieldCustom.ini в вашу версию этого файла.

**Убрать Message Of The Day**

+ Правка файла "StarfieldCustom.ini".
+ В секции [General] добавьте параметр "bEnableMessageOfTheDay=0" без кавычек.

## Функционал

**Настроить FOV камеры**

+ Правки файла "StarfieldCustom.ini".
```
[Display]
fDefaultFOV=100.0

[Camera]
fFPWorldFOV=100.0
fTPWorldFOV=100.0

[FlightCamera]
fFlightCameraFOV=100.0

[Dialogue]
; установка FOV в диалогах
fDialogueCameraCollisionMinPercentage=3.5
fDialogueCameraCollisionRadius=3.5
fDialogueCameraFailsafeFPFOV=75.0
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

**Вменяемое прилипание в строительстве**

+ Правки файла "StarfieldCustom.ini".
```
[Workshop]
fWorkshopItemConnectPointQueryRadius=0.35
fWorkshopItemWouldBeSnappedDistance=0.30
fWorkshopBreakSnapRadiusMult=0.5
fOutpostSnapPreviewHoldSnappedTime=-50.0
fOutpostSnapPreviewWaitForPreviewTime=-50.0
fOutpostSnapWaitForPostSnapCycleTime=-50.0
; перекрытие объектов
fClosestPointToleranceLargeItems=-100.0
```

**Быстрое перетаскивание предметов**

+ Правки файла "StarfieldCustom.ini".
```
[Controls]
fQCZKeyDelay=0.15
fZKeyDelay=0.15
```

**Увеличить количество авто-сохранений**

+ Правка файла "StarfieldCustom.ini".
+ В секции [SaveGame] добавьте параметр "iAutoSaveCount=20" без кавычек.

**Джетпак через удержание клавиши**

+ Правка файла "StarfieldCustom.ini".
+ В секции [Boostpack] добавьте параметр "bUsePressAndHoldControls=1" без кавычек.

**Горячие клавиши для консольных команд**

+ Правка файла "StarfieldCustom.ini".
+ В секции [Menu] добавьте параметр "bUseConsoleHotkeys=1" без кавычек.
+ Создайте файл "StarfieldConsole.ini" по адресу "Документы/My Games/Starfield/StarfieldConsole.ini".
+ Добавьте в новый файл секции [Macros] и [Hotkeys], а также настройки клавиш и команд.

```
[Macros]
heal=Player.RestoreAV Health 5000.0
kill=Player.Kill

[Hotkeys]
F1=ShowMenu SleepWaitMenu
F2=bat "My-Bat-File"
F3=heal;kill
F4=qqq
```

## Графика

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

**Заменить FSR2 на DLSS и Nvidia Reflex**

+ Установите [Streamline Native](https://www.nexusmods.com/starfield/mods/2751) как обычный мод в MO2.
+ Скачайте файлы "[nvngx_dlss.dll](https://www.techpowerup.com/download/nvidia-dlss-dll/)" и "[nvngx_dlssg.dll](https://www.techpowerup.com/download/nvidia-dlss-3-frame-generation-dll/)".
+ Скопируйте их в папку "SFSE\Plugins\nv-streamline" мода Streamline Native.

    <details><summary>Структура мода после всех действий должна выглядеть так.</summary><p>

    ![](Как-сделать-X/Streamline-Native.png)

    </p></details>

+ При этом не забудьте поставить мод [Upscaling Fix 2](https://www.nexusmods.com/starfield/mods/3930), который убирает мерцание ткани при любом апскейле.

**Заменить внешность NPC**

1. Разместите рядом с собой "мусорного" NPC своего пола.
    + player.placeatme 50566 1 ; женщина
    + player.placeatme 5055F 1 ; мужчина
2. Выберите его в консоли (должен быть тип "NPC_", ID FFXXXXXX) и запомните его ID.
3. Используйте консольную команду "capp 14", чтобы перенести внешность ГГ на "мусорного" NPC.
4. Используйте консольную команду "slm 14", чтобы открыть редактор внешности ГГ.
5. Измените внешность ГГ так, как вам хочется, и подтвердите изменения.
6. Выберите в консоли нужного вам NPC (должен быть тип "NPC_", ID XXYYYYYY) и используйте консольную команду "capp 14", чтобы перенести на него внешность ГГ.
7. Выберите в консоли ГГ (должен быть тип "NPC_", ID 00000014) и используйте консольную команду "capp ID", где ID - это ID "мусорного" NPC из пункта 2.
8. Выберите в консоли "мусорного" NPC и используйте команды "Disable" и "MarkForDelete", чтобы стереть его.

## Прочее

**Добавить трейты на экипировку**

+ Выбросьте предмет на землю и выберите его в консоли. Можно использовать скролл мышью.

<details><summary>Для брони должен быть тип ARMO, ID FFXXXXXX. Используйте консольную команду AMod.</summary><p>

Базовое качество брони влияет на боевые защитные характеристики.

```
﻿11E2BB    mod_Armor_Spacesuit_Quality_01
11E2BC    mod_Armor_Spacesuit_Quality_02
11E2BA    mod_Armor_Spacesuit_Quality_03
11E2B9    mod_Armor_Spacesuit_Quality_04
03AF7D    mod_Armor_Spacesuit_Quality_05

11E2B5    mod_Armor_Helmet_Quality_01
11E2B6    mod_Armor_Helmet_Quality_02
11E2B7    mod_Armor_Helmet_Quality_03
11E2B8    mod_Armor_Helmet_Quality_04
03AF80    mod_Armor_Helmet_Quality_05

1CAE05    mod_Armor_Backpack_Quality_01
1CAE34    mod_Armor_Backpack_Quality_02
1CAE35    mod_Armor_Backpack_Quality_03
1CAE36    mod_Armor_Backpack_Quality_04
03AF7F    mod_Armor_Backpack_Quality_05
```

Также у брони есть планетарные защитные характеристики.

```
0E9A8D    mod_Armor_Spacesuit_ENV_Airborne04
112173    mod_Armor_Spacesuit_ENV_Corrosive04
113578    mod_Armor_Spacesuit_ENV_Radiation04
11B756    mod_Armor_Spacesuit_ENV_Thermal04
1AEB51    mod_Armor_Spacesuit_ENV_Balanced01

0DDCE7    mod_Armor_Helmet_ENV_Airborne04
112154    mod_Armor_Helmet_ENV_Corrosive04
1124D1    mod_Armor_Helmet_ENV_Radiation04
11B747    mod_Armor_Helmet_ENV_Thermal04
1AEB57    mod_Armor_Helmet_ENV_Balanced01

1C1DF5    mod_Armor_Backpack_ENV_Airborne04
1C1DFD    mod_Armor_Backpack_ENV_Corrosive04
1C1E01    mod_Armor_Backpack_ENV_Radiation04
1C1E05    mod_Armor_Backpack_ENV_Thermal04
1C1DF6    mod_Armor_Backpack_ENV_Balanced01

2C38BF    mod_Armor_Spacesuit_ENV_Starborn01    Уникальный бонус, который стакается с любым из бонусов выше.
```

</p></details>

<details><summary>Эта же команда может добавлять броне трейты, максимум 3 трейта, по одному из каждой группы.</summary><p>

```
Скафандры, Группа 1

Chameleon         1336C1﻿    Blend with the environment while sneaking and not moving.
Bolstering        1336C6﻿    Grants up to +100 Energy resistance and Physical resistance, the lower your health.
Anti-Ballistic    13369E﻿    -15% incoming Physical damage from ranged weapons.
Beast Hunter      1336BD﻿    -15% damage from Alien enemies.
Ablative          13369C﻿    -15% incoming Energy damage.
Combat Veteran    1336BE﻿    -15% damage from Human enemies.
Sturdy            133699﻿    -15% incoming melee damage.
Technician        1336BC﻿    -15% damage from Robot enemies.

Скафандры, Группа 2

Auto-Medic         0C9A43﻿    Automatically use a Med Pack when hit and health is below 25%, once every 60 seconds.
Resource Hauler    060293﻿    Resources weigh 25% less.
Weapon Holsters    060295    Weapons weigh 50% less.
Antiseptic         0710FA﻿    +25 Airborne Resistance.
Galvanized         0710F7﻿    +25 Corrosive Resistance.
Leadlined          0710F5﻿    +25 Radiation Resistance.
Liquid Cooled      0710F6﻿    +25 Thermal Resistance.
Acrobat            0710FD﻿    -50% fall damage.

Скафандры, Группа 3

Mechanized    0BE542﻿    +40 carry capacity.
Repulsing     06029d﻿    5% chance to disarm nearby attackers.
Incendiary    002983﻿    10% chance to ignite nearby attackers.
Sentinel      0BE540﻿    75% chance to reduce damage by 50% while standing still.
Peacemaker    2D01A2    Rifles do 10% more damage.
Mirrored      059AE8﻿    4% chance to reflect attacks.
Reactive      06029F﻿    10% chance to stagger nearby attackers.

Шлемы, Группа 1

> Доступны трейты скафандров + 2 уникальных
O2 Boosted    0690B0    +20% oxygen capacity.
O2 Filter     0690AE    -25% oxygen consumption.

Шлемы, Группа 2

> Доступны трейты скафандров + 2 уникальных
Hacker      2C43DA    +2 max auto attempts that can be banked while hacking.
Analyzer    0690AF    +10% damage to scanned targets.

Шлемы, Группа 3

> Доступны трейты скафандров + 2 уникальных
Sensor Chip    2C43DB    +20% accuracy while firing on the move.
Headhunter     2C43DC    Deals +25% damage on the next attack after hitting a target's head.

Джетпаки, Группа 1

> Доступны трейты скафандров

Джетпаки, Группа 2

> Доступны трейты скафандров + 1 уникальный
Fastened    2EDE4E    +20 carry capacity.

Джетпаки, Группа 3

> Доступны трейты скафандров + 2 уникальных
Armor-Plated      2EDE59    -10% incoming Physical, Energy, and EM damage.
Assisted Carry    2EDE4F    Drain 75% less O2 when running while encumbered.
```

</p></details>

<details><summary>С оружием всё работает точно так же, но тип должен быть WEAP.</summary><p>

```
Оружие, Группа 1

Anti-Personnel       0FF442    +10% damage against humans.
Bashing              0FEA07    Deals double damage when gun bashing.
Berserker            0F437E    Does more damage the less armor one has.
Cornered             0F428E    Damage increases as health decreases.
Disassembler         1625EB    +20% damage against robots. 
Extended Magazine    0FFA3B    Doubles the base magazine capacity.
Exterminator         15DD18    +30% damage against aliens.
Furious              0EA117    Each consecutive hit deals more damage.
Instigating          0F2013    Deals double damage to targets with full health.
Oxygenated           0FAEAB    Hold-breath time when aiming using a scoped weapon is increased.
Space-Adept          0F7321    +30% damage while in space, and -15% damage while on a planet.

Оружие, Группа 2

Corrosive      08AB47    Randomly deals corrosive damage and reduces the targets' armor over 6 seconds.
Crippling      0F2E39    Deals +30% damage on the next attack after hitting a target's limbs.
Handloading    0EA0BA    Volatile rounds that are designed to pack a bigger punch, but aren't as stable and can fail on occasion.
Hitman         122F1C    +15% damage while aiming.
Incendiary     07D728    Randomly deals incendiary damage.
Lacerate       0FEA49    Randomly applies a bleed effect to the target.
Med Theft      0FFA3C    Chance that humans drop extra Med Packs on death.
Poison         319AEC    Randomly deals poison damage and slows the target.
Radioactive    0EA13B    Randomly deals radioactive damage and demoralizes the target.
Rapid          0FEA04    +25% increase in attack speed.
Staggering     0E8D64    Small chance to stagger enemies.

Оружие, Группа 3

Concussive        0FBD3C    Small chance to knock down targets.
Demoralizing      0FC884    Small chance to demoralize a target.
Elemental         31C0C5    Randomly deals Corrosive, Radiation, Poison, and Incendiary damage.
Explosive         0FA8D6    Randomly switches to explosive rounds.
Frenzy            0FC8A4    Small chance to frenzy a target.
One Inch Punch    0F4CF0    Rounds fire in a shotgun-like spread.
Shattering        0F4557    Break through even the strongest armor.
Skip Shot         31C0C4    Every fourth shot fires two projectiles at once.
Tesla             31C0C6    Rounds will sometimes emit electricity where they land that damages and slows nearby targets.
Titanium Build    0FFA3D    Premium build materials make this weapon light as a feather.
```

</p></details>

+ Для удаления модификатора используйте аналогичную команду RMod.

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

------

|[*Назад к оглавлению*](https://github.com/Meridiano/Starfield-Head)|
|:---:|