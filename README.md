# SenkoPets - Pet Taming with a Friendship System

**A plugin that expands vanilla pet taming with a progressive friendship system and full pet management.** Tame seven pets, raise their friendship level, unlock unique abilities and control every pet from a convenient GUI.

**This plugin is under active development** - new features are on the way. Stay tuned for the **Versions** section!

## Features

- **7 tameable pets**: Cat, Dog (Wolf), Fox, Panda, Polar Bear, Frog, Armadillo
- **Friendship system** with 5 levels - feed and pet your pets to raise friendship
- **Level bonuses**: extra maximum health, extra damage, passive regeneration
- **Unique species abilities**, including the Armadillo's active ability
- **Follow / Stay** modes, no despawn, teleport to the owner over long distances
- **Pet GUI** to view and manage each pet
- **Pet list**, renaming with color codes, transfer to other players, release
- **Configurable** taming items, favorite foods, friendship points, cooldowns and pet limits
- **Permission system**: senkopets.use, senkopets.extended, senkopets.admin
- **Languages**: Russian and English

## Taming

Right-click an animal while holding its taming item:

| Pet | Taming item |
|---|---|
| Fox | Sweet Berries |
| Polar Bear | Raw Cod / Raw Salmon |
| Panda | Bamboo |
| Frog | Spore Blossom |
| Armadillo | Spider Eye |
| Cat | Raw Cod / Raw Salmon |
| Dog (Wolf) | Bone |

Tamed pets no longer despawn.

## Friendship System

**Feed** your pet its favorite food (right-click while holding it): **+15 FP**, cooldown 5 minutes.
**Pet** your pet (Shift + right-click with an empty hand): **+10 FP**, cooldown 3 minutes.

### Levels

| Level | Points | Bonus |
|---|---|---|
| 1 | 0 | Basic commands, no despawn |
| 2 | 50 | +20% to maximum health |
| 3 | 125 | +25% to damage dealt |
| 4 | 225 | Regeneration - 1 HP every 10 seconds |
| 5 | 375 | Unique species ability |

Maximum friendship: **575 points**.

### Unique abilities

| Pet | Level | Ability |
|---|---|---|
| Fox | 2 | 10% chance to drop Sweet Berries from killed chickens |
| Polar Bear | 3 | 25% chance to apply Weakness I (3 s) on hit |
| Panda | 4 | Gifts 1–3 Bamboo every 10 minutes |
| Frog | 4 | Creates a Regeneration zone (5 s, radius 3 blocks) for the owner every 2 minutes |
| Armadillo | 5 | **/pet ability** - rolls into a ball with Resistance II for 8 seconds (60 s cooldown) |

## Companion Menu

Open the pet's menu with **/pet stats** while looking at it, or click the pet in the list (**/pet**). The menu shows the pet's head, type, owner, friendship level and mode, and gives access to **Rename**, **Transfer** and **Release** buttons.

## Commands

| Command | Description | Permission |
|---|---|---|
| /pet | Open your pet list | senkopets.use |
| /pet stats | Open the menu of the pet you are looking at (up to 10 blocks) | senkopets.use |
| /pet follow | The pet you look at starts following you | senkopets.use |
| /pet stay | The pet you look at stays in place | senkopets.use |
| /pet ability | Use the Armadillo's ball form (level 5) | senkopets.use |
| /pet transfer \<player\> | Transfer a pet to another player | senkopets.use |
| /pet rename \<name\> | Rename a pet (costs experience levels, supports color codes) | senkopets.extended |
| /pet release [confirm] | Release a pet - confirm within 20 seconds | senkopets.extended |
| /pet all follow / stay | Apply the mode to all your pets within 50 blocks | senkopets.extended |
| /pet help | Show the command list | senkopets.use |
| /pet reload | Reload config and language files | senkopets.admin |

**Transfer cooldown**: 24 hours for senkopets.use, **15 minutes** for senkopets.extended.

## Permissions

| Permission | Default | Description |
|---|---|---|
| senkopets.use | Everyone | Basic access: commands, taming, feeding, petting, pet list |
| senkopets.extended | Nobody | Rename, release, all-modes; faster transfer cooldown |
| senkopets.admin | Operators | /pet reload |

`senkopets.extended` inherits `senkopets.use`; `senkopets.admin` inherits `senkopets.extended`.

## Configuration

The plugin creates **config.yml** with settings for:

- taming items and favorite foods per species
- friendship points and cooldowns (feeding, petting)
- transfer cooldowns (use / extended)
- maximum pets per player
- species ability toggles (on/off)
- language selection

Messages are stored in the **language/** folder as **ru.yml** and **en.yml** and are fully editable.

---

**Attention!** The plugin is under active development - functionality is being added and improved. Follow the **Versions** section for updates.

**Join our Minecraft server:** [SenkoSan](https://modrinth.com/server/senkosan)

---

# SenkoPets - Приручение питомцев с системой дружбы

**Плагин, который расширяет стандартное приручение животных прогрессивной системой дружбы и полным управлением питомцами.** Приручайте семь питомцев, повышайте уровень дружбы, открывайте уникальные способности и управляйте каждым питомцем через удобное меню.

**Плагин находится в активной разработке** - новые функции уже в пути. Следите за разделом **«Версии»**!

## Требования

- **Дата-пак**: [Mob Heads](https://modrinth.com/datapack/mob-heads) - нужен для корректного отображения голов мобов в меню плагина.

## Возможности

- **7 приручаемых питомцев**: кошка, собака (волк), лиса, панда, белый медведь, лягушка, броненосец
- **Система дружбы** из 5 уровней - кормите и гладьте питомцев, чтобы повышать дружбу
- **Бонусы уровней**: больше здоровья, больше урона, пассивная регенерация
- **Уникальные способности** видов, включая активную способность броненосца
- **Режимы Следовать / Оставаться**, отсутствие деспавна, телепортация к владельцу на больших расстояниях
- **GUI питомца** для просмотра и управления
- **Список питомцев**, переименование с цветовыми кодами, передача другим игрокам, отпускание на волю
- **Настройка** предметов приручения, любимой еды, очков дружбы, перезарядок и лимита питомцев
- **Система прав**: senkopets.use, senkopets.extended, senkopets.admin
- **Языки**: русский и английский

## Приручение

Нажмите ПКМ по животному, держа в руке предмет приручения:

| Питомец | Предмет приручения |
|---|---|
| Лиса | Сладкие ягоды |
| Белый медведь | Сырая треска / Сырой лосось |
| Панда | Бамбук |
| Лягушка | Сливово-розовый лист |
| Броненосец | Паучий глаз |
| Кошка | Сырая треска / Сырой лосось |
| Собака (волк) | Кость |

Прирученные питомцы больше не деспавнятся.

## Система дружбы

**Покормите** питомца любимой едой (ПКМ, держа еду в руке): **+15 очков**, перезарядка 5 минут.
**Погладьте** питомца (Shift + ПКМ пустой рукой): **+10 очков**, перезарядка 3 минуты.

### Уровни

| Уровень | Очки | Бонус |
|---|---|---|
| 1 | 0 | Базовые команды, отсутствие деспавна |
| 2 | 50 | +20% к максимальному здоровью |
| 3 | 125 | +25% к наносимому урону |
| 4 | 225 | Регенерация - 1 HP каждые 10 секунд |
| 5 | 375 | Уникальная способность вида |

Максимум дружбы: **575 очков**.

### Уникальные способности

| Питомец | Уровень | Способность |
|---|---|---|
| Лиса | 2 | 10% шанс выпадения сладких ягод с убитой курицы |
| Белый медведь | 3 | 25% шанс наложить Слабость I (3 сек) при ударе |
| Панда | 4 | Дарит 1–3 бамбука каждые 10 минут |
| Лягушка | 4 | Создаёт зону Регенерации (5 сек, радиус 3 блока) для владельца каждые 2 минуты |
| Броненосец | 5 | **/pet ability** - сворачивается в шар с Сопротивлением II на 8 секунд (перезарядка 60 сек) |

## Меню питомца

Откройте меню питомца командой **/pet stats**, глядя на него, или нажав на питомца в списке (**/pet**). Меню показывает голову, тип, владельца, уровень дружбы и режим питомца, а также даёт доступ к кнопкам **Переименовать**, **Передать** и **Отпустить**.

## Команды

| Команда | Описание | Право |
|---|---|---|
| /pet | Открыть список ваших питомцев | senkopets.use |
| /pet stats | Открыть меню питомца, на которого вы смотрите (до 10 блоков) | senkopets.use |
| /pet follow | Питомец под прицелом начинает следовать за вами | senkopets.use |
| /pet stay | Питомец под прицелом остаётся на месте | senkopets.use |
| /pet ability | Использовать способность броненосца (5 уровень) | senkopets.use |
| /pet transfer \<игрок\> | Передать питомца другому игроку | senkopets.use |
| /pet rename \<имя\> | Переименовать питомца (стоит уровней опыта, поддерживает цветовые коды) | senkopets.extended |
| /pet release [confirm] | Отпустить питомца - подтвердите в течение 20 секунд | senkopets.extended |
| /pet all follow / stay | Применить режим ко всем вашим питомцам в радиусе 50 блоков | senkopets.extended |
| /pet help | Показать список команд | senkopets.use |
| /pet reload | Перезагрузить конфиг и языковые файлы | senkopets.admin |

**Перезарядка передачи**: 24 часа для senkopets.use, **15 минут** для senkopets.extended.

## Права доступа

| Право | По умолчанию | Описание |
|---|---|---|
| senkopets.use | Все | Базовый доступ: команды, приручение, кормление, поглаживание, список питомцев |
| senkopets.extended | Никто | Переименование, отпускание, режимы «все»; уменьшенная перезарядка передачи |
| senkopets.admin | Операторы | /pet reload |

`senkopets.extended` наследует `senkopets.use`; `senkopets.admin` наследует `senkopets.extended`.

## Конфигурация

Плагин создаёт **config.yml** с настройками:

- предметы приручения и любимая еда для каждого вида
- очки и перезарядки дружбы (кормление, поглаживание)
- перезарядки передачи (use / extended)
- максимальное количество питомцев на игрока
- включение/отключение способностей видов
- выбор языка

Сообщения хранятся в папке **language/** в файлах **ru.yml** и **en.yml** и полностью редактируются.

---

**Внимание!** Плагин находится в активной разработке - функционал дополняется и улучшается. Следите за обновлениями в разделе **«Версии»**.

**Заходите на наш Minecraft-сервер:** [SenkoSan](https://modrinth.com/server/senkosan)
~~~~
