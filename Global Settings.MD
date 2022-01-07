Global Settings 
Global settings affect all worlds on the server as well as the core server functionality itself.

verbose 
default: false
description: 设置服务器是否应该将所有配置值转储到启动时的服务器日志
config-version 
没有任何原因改变这个！这是在内部使用的，以帮助自动更新您的配置
command 
uptime 
format 
default: "<days><hours><minutes><seconds>"
description: <uptime>占位符用于uptime-command-output的格式
日
default: "%02d day, "
description: 命令<day>占位符的输出.uldime.format选项
天
default: "%02d days, "
description: <days>占位符的输出命令.uldime.format选项
小时
default: "%02d hour, "
description: 命令中<小时>占位符的输出.uldime.format选项
小时
default: "%02d hours, "
description: 命令中的<小时>占位符的输出.uldime.format选项
分钟
default: "%02d minute, and "
description: Command.uptime.format选项中<mime>占位符的输出
分钟
default: "%02d minutes, and "
description: <分钟>占位符的输出.uldime.format选项
第二
default: "%02d second"
description: <秒>占位符的输出命令.uldime.format选项
秒
default: "%02d seconds"
description: <秒>占位符的输出.uldime.format选项
游戏模式
requires-specific-permission 
Requires minecraft.command.gamemode.<gamemode> permission
default: false
description: 为每个GameMode设置为TRUE要求自己的许可
TPSBar.
title 
<tps> - The current TPS

<mspt> - The current MSPT

<ping> - The current ping

default: <gray>TPS<yellow>:</yellow> <tps> MSPT<yellow>:</yellow> <mspt> Ping<yellow>:</yellow> <ping>ms
description: 当/ tpsbar命令运行时，bossbar的格式
覆盖
default: NOTCHED_20
description: 设置Bossbar的叠加类型
Available options: PROGRESS, NOTCHED_6, NOTCHED_10, NOTCHED_12, NOTCHED_20
fill-mode 
default: MSPT
description: Bossbar Bar应显示可用选项：TPS，MSPT，Ping
进步颜色 
Available options: PINK, BLUE, RED, GREEN, YELLOW, PURPLE, WHITE

good 
default: GREEN
description: 填充模式是“好”时应该显示的颜色
medium 
default: YELLOW
description: 填充模式是“中等”时应该显示哪种颜色
low 
default: RED
description: 填充模式为“低”时应显示哪种颜色
text-color 
<text> - 来自setings.command.tpsbar.title的格式

good 
default: <gradient:#55ff55:#00aa00><text></gradient>
description: <text>填充模式为“好”时的梯度
medium 
default: <gradient:#ffff55:#ffaa00><text></gradient>
description: 填充模式为“中”时<text>的梯度
low 
default: <gradient:#ff5555:#aa0000><text></gradient>
description: 填充模式为“低”时<text>的梯度
tick-interval 
default: 20
description: Bossbar应该更新频率
compass 
title 
default: "S · ◈ · ◈ · ◈ · SW · ◈ · ◈ · ◈ · W · ◈ · ◈ · ◈ · NW · ◈ · ◈ · ◈ · N · ◈ · ◈ · ◈ · NE · ◈ · ◈ · ◈ · E · ◈ · ◈ · ◈ · SE · ◈ · ◈ · ◈ ·
S · ◈ · ◈ · ◈ · SW · ◈ · ◈ · ◈ · W · ◈ · ◈ · ◈ · NW · ◈ · ◈ · ◈ · N · ◈ · ◈ · ◈ · NE · ◈ · ◈ · ◈ · E · ◈ · ◈ · ◈ · SE · ◈ · ◈ · ◈ · "
description: 当/ compass命令是ran时，bossbar的格式
overlay 
default: PROGRESS
description: 设置Bossbar的叠加类型
Available options: PROGRESS, NOTCHED_6, NOTCHED_10, NOTCHED_12, NOTCHED_20
progress-color 
Available options: PINK, BLUE, RED, GREEN, YELLOW, PURPLE, WHITE

default: GREEN
description: Bossbar的颜色
percent 
default: 1.0
description:Bossbar如何覆盖0.0到1.0
tick-interval 
default: 5
description:Bossbar应该更新频率
hide-hidden-players-from-entity-selector 
default: false
description: 设置为true以隐藏实体选择器中的玩家
allow-water-placement-in-the-end 
default: true
description: 允许将水放置在最后。
dont-send-useless-entity-packets 
default: false
description: 跳过发送没有真正移动的实体的相对移动数据包
Warning
已知unt-send-unless-entity-packets选项选项会导致安装某些插件的问题，尤其是选项卡和同伴。

use-alternate-keepalive 
default: false
description: 使用不同的方法来保持keepalive ping超时。启用这一点向玩家发送一次KeepAlive数据包，并且只有在30秒内响应时，才能踢超时。以任何顺序响应其中任何一个都将保持玩家连接。又名，它不会踢你的球员，因为1个数据包在沿线的某个地方丢弃
tps-catchup 
default: true
description: 控制TPS追赶
Note
TPS Captup在任何时间后，您的服务器刻度会在20以下的任何时间后比20 TPS更快。这是一种尽可能接近20的平均TPS尝试，但确实含有自己的副作用

server-mod-name 
default: Purpur
description: 这会修改在客户端过时或某人打开调试屏幕时显示的服务器名称 [F3]
lagging-threshold 
default: 19.0
description: PURPUR在滞后时，追踪措施，以便相应地改变行为的能力。当您想考虑服务器滞后时，此值是该阈值。现在这仅用于mob.villager.brain-ticks设置
disable-give-dropping 
default: false
description: 设置为true以禁用/授予命令在玩家的库存已满时丢弃地板上的项目
messages 
Afk-Broadion
要求踢踢 -  ifle设置为false

default: §e§o%s is now AFK
description: 这是当用户转到AFK时被广播的消息（必须具有大于0和kick-if-idle设置为false的播放器 - 空闲时间设置为false）
afk-broadcast-back 
Requires the kick-if-idle setting to be false

default: §e§o%s is no longer AFK
description: 这是当用户不再AFK时广播的消息（必须具有大于0和kick-if-idle设置为false的播放器空闲 - 超时设置为false）
afk-tab-list-prefix 
Requires the kick-if-idle setting to be false

default: "[AFK] "
description: 在他们的名字之前在玩家列表上显示的前缀
afk-tab-list-suffix
Requires the kick-if-idle setting to be false

default: ""
description: 在他们的名字之后出现在玩家列表上的后缀
ping-command-output 
Requires the bukkit.command.ping permission

default: §a%s's ping is %sms
description: 运行/ ping <user>时输出。
cannot-ride-mob 
Requires the allow.ride.<mob_id> permission

default: §cYou cannot mount that mob
description: 显示当有人尝试安装暴徒时显示的消息他们不允许。
uptime-command-output 
Requires the bukkit.command.uptime permission <uptime> - The format from <global>.command.uptime.format

default: <green>Server uptime is <uptime>
description: 显示/ uptime命令运行时显示的消息。
dont-run-with-scissors 
Requires the damage-if-sprinting option to be enabled

default: <red><italic>Don't run with scissors!
description: actionbar消息显示何时有人attempts to run with scissors
demo-command-output 
Requires the bukkit.command.demo permission

default: §a%s has been shown the demo screen
description: 显示演示屏幕的消息 enabled for a user using the /demo command.
credits-command-output 
Requires the bukkit.command.credits permission

default: §a%s has been shown the end credits
description:显示使用/ cccits命令启用贷记屏幕时的消息。
unverified-username 
default: default
description: 显示播放器当播放器被踢出未经验证的用户名时（用户处于离线模式）。设置为“默认”显示默认消息“无法验证用户名！”
sleep-skipping-night 
default: default
description: 跳过夜晚时出现的动作栏消息。设置为“默认”以让客户端使用自己的可翻译组件。设置为空字符串以禁用它。
sleeping-players-percent 
default: default
description: 播放器睡着时出现的动作栏消息。设置为“默认”以让客户端使用自己的可翻译组件。设置为空字符串以禁用它。可用占位符：<count>  - 当前的玩家睡眠量，<总>  - 睡眠所需的球员总量
network 
upnp-port-forwarding 
default: false
description: 当服务器启动时，尝试使用UPnP自动转发
blocks 
barrel 
rows 
default: 3
description: 桶的行数应该有。Min：1，Max：6
beehive 
max-bees-inside 
default: 3
description: 蜂箱里面允许的蜜蜂的最大数量/ bee_nest
grindstone 
ignore-curses 
default: true
description: 设置为false以允许磨石从物品中删除诅咒魅力
ender_chest 
six-rows 
default: false
description: 柜内箱应该有六排库存空间
use-permissions-for-rows 
Requires ender_chest.six-rows to be true
Requires purpur.enderchest.rows.<number> permission
default: false
description: 使用权限节点来确定行的数量。默认情况下，除非启用此设置，否则除非使用权限另有指定，否则所有播放器都有六行。
禁用 - 蘑菇 - 更新
default: false
description: 从更新它的块状态服务器端停止蘑菇块
disable-chorus-plant-updates 
default: false
description: 从更新它的块状态服务器端停止合唱工厂
disable-note-block-updates 
default: false
description: 从更新它的块状态服务器端停止注释块
crying_obsidian 
valid-for-portal-frame 
default: false
description: 设置为true以使您可以在哭泣的黑曜石中创建门户
broadcasts 
advancement 
only-broadcast-to-affected-player 
default: false
description: 仅广播聊天的前进消息仅在受影响的播放器中
death 
only-broadcast-to-affected-player 
default: false
description: 仅向受影响的播放器聊天中的死亡消息
logger 
suppress-init-legacy-material-errors 
default: false
description: 抑制关于插件初始化遗留的警告material api
suppress-ignored-advancement-warnings 
default: false
description: 在控制台和日志中抑制关于未知属性的警告
suppress-unrecognized-recipe-errors 
default: false
description: 抑制有关装载无法识别的配方的尝试的警告
seed 
structure 
Check out https://minecraft.fandom.com/wiki/Custom_world_generation#Structure_defaults 有关下面选项的更多信息

buried_treasure 
default: -1
description:默认值为-1“使用世界种子”。什么都不是-1将是一种定制种子。它可以接受任何整数值（-2147483648至2147483647）
mineshaft 
default: -1
description: 默认值为-1“使用世界种子”。什么都不是-1将是一种定制种子。它可以接受任何整数值（-2147483648至2147483647）
stronghold 
default: -1
description: The default value is -1 for "use the world seed". anything not -1 will be a custom seed. it can accept any Integer value (-2147483648 to 2147483647)
entity 
enderman 
short-height 
default: false
description: 如果启用，允许Endermen拟合成2个块高空间。由于客户端的Hitbox保持不变，因此您仍然可以在头部击中它们
enchantment 
allow-infinity-and-mending-together 
default: false
description: 允许修补和无穷大附加在同一武器/工具上
allow-infinity-on-crossbow 
default: false
description: 允许对弩上的无限魅力
allow-unsafe-enchants 
default: false
description:允许增加魔法的能力通过了最大水平
World Settings 
世界环境是均为世界的。子节点默认值用于所有没有自己特定设置的世界

hunger 
starvation-damage 
default: 1.0
description: 伤害饥饿的数量将会做到
块
dragon_egg 
teleport 
default: true
description: 在击中时控制龙蛋是否会传送
amethyst 
silk-touch 
default: false
description: 是否可以通过用丝绸触摸迷住的物品来捡起紫水晶
observer 
disable-clock 
default: false
description: disable observer clocks
azalea 
growth-chance 
default: 0.0
description: 杜鹃花的机会自然地成长为树木
flowering_azalea 
growth-chance 
default: 0.0
description: 开花杜鹃花的机会成长为树木 naturally
campfire 
lit-when-placed 
default: true
description: 设置为false以停止在放置时点燃篝火
cactus 
breaks-from-solid-neighbors 
default: true
description: 仙人掌是否将从它旁边的固体块中断
cauldron 
fill-chances 
rain 
default: 0.05
description: 大锅填充雨的速度（取决于随机蜱虫）
powder-snow 
default: 0.1
description: 大锅用粉末雪充填的速度（取决于随机蜱）
turtle_egg 
break-from-exp-orbs 
default: true
description: 允许EXP ORBS损坏/断龟蛋
break-from-items 
default: true
description:允许掉落的物品损坏/脱龟蛋
break-from-minecarts 
default: true
description: 让Minecarts损坏/脱龟蛋
bypass-mob-griefing 
default: false
description:为龟蛋绕过暴徒的真实griefing gamerule
powered-rail 
activation-range 
default: 8
description: 由单个redstone源激活的动力轨道的数量
conduit 
valid-ring-blocks 
default:

- minecraft:prismarine
- minecraft:prismarine_bricks
- minecraft:sea_lantern
- minecraft:dark_prismarine
default:
description:可用于构建导管的块
effect-distance 
default: 16
description: 框架中每七个块的导管的有效半径
mob-damage 
distance 
default: 8
description:距离敌对暴徒的距离（块）
damage-amount 
default: 4
description: 如果它们与水/雨接触，每2秒适用于敌对暴徒的损害金额
beacon 
effect-range 
level-1 
default: 20
description: 块的数量效果范围达到此级别
level-2 
default: 30
description: Amount of blocks the effect range reaches for this level
level-3 
default: 40
description: Amount of blocks the effect range reaches for this level
level-4 
default: 50
description: 块的数量效果范围达到此级别
sponge 
absorbs-lava 
default: false
description: 设置为true以允许海绵吸收熔岩
absorption 
area 
default: 64
description:海绵吸收水的块区域
radius 
default: 6
description: 海绵吸收水的块半径
composter 
sneak-to-bulk-process 
default: false
description: 设置为TRUE，以便通过潜行右键单击手中的物品批量处理食品/植物物品
slab 
break-individual-slabs-when-sneaking 
default: false
description: 设置为true，以允许在偷偷静时打破双层块中的单个板块
packed_ice 
allow-mob-spawns 
default: true
description: 设置为false以禁用包装冰块的暴徒
blue_ice 
allow-mob-spawns 
default: true
description: 设置为false，以禁用蓝冰的暴针
sand 
fix-duping 
default: true
description: 设置为false以重新启用沙欺骗的能力
end_portal 
safe-teleporting 
default: true
description: 在处理结束门户传送中，将保护免受不安全代码的保护。某些漏洞可能需要禁用这一点
dispenser 
apply-cursed-to-armor-slots 
default: true
description: 如果迷人的绑定诅咒，请分配器将装甲涂抹在装甲插槽中
respawn_anchor 
explode 
default: true
description: 是否重新锚爆炸。将此设置为false只是使重生锚挖掘出存在
explosion-power 
default: 5.0
description: 爆炸半径的爆炸半径。（相比之下，TNT是4.0，而且收费爬行物为6.0）
explosion-fire 
default: true
description:爆炸是否会导致火灾
explosion-effect 
default: DESTROY
description: 如何处理受爆炸影响的块。销毁将破坏块（没有项目滴）。突破自然会破坏块（物品将掉落）。没有人不会破坏任何街区
sign 
allow-colors 
Requires purpur.sign.color, purpur.sign.style, and/or purpur.sign.magic permission
default: false
description: 允许玩家在符号上使用颜色代码
right-click-edit 
Requires purpur.sign.edit permission
default: false
description:能够通过右键单击其另一个签名来编辑符号
magma-block 
damage-when-sneaking 
default: false
description: 设置为true以在偷偷时损坏
damage-with-frost-walker 
default: false
description: 设置为true，以在与冰霜漫步的靴子一起散步时造成伤害
lava 
infinite-source 
default: false
description: 允许熔岩采取类似于水的无限供应特性（<无限必需 - 源>流动的源块创建一个新的源块）
infinite-required-sources 
default: 2
description: 具有无限熔岩所需的来源量
speed 
nether 
default: 10
description: 物理/流动之间的瞬间延迟（更低的速度）
not-nether 
default: 30
description: Delay in ticks between physics/flowing (lower is faster)
water 
infinite-source 
default: true
description:设置如果水应该具有无限属性（<无限的所需源>流动的源块创建一个新的源块）
infinite-required-sources 
default: 2
description:具有无限水所需的来源量
piston 
block-push-limit 
default: 12
description: 活塞的块数量可以推动
bed 
explode 
default: true
description: 床是否爆炸。将此设置为false只是使床结合出存在
explode-on-villager-sleep 
default: false
description: 村庄睡觉时床是否爆炸。
explosion-power 
default: 5.0
description: 爆炸半径的爆炸半径。（相比之下，TNT是4.0，而且收费爬行物为6.0）
explosion-fire 
default: true
description: 爆炸是否会导致火灾
explosion-effect 
default: DESTROY
description: 如何处理受爆炸影响的块。销毁将破坏块（没有项目滴）。突破自然会破坏块（物品将掉落）。没有人不会破坏任何街区
farmland 
get-moist-from-below 
default: false
description: 让土壤直接下方从水中滋润水
use-alpha-farmland 
default: false
description: 如果栅栏或鹅卵石直接放在它下面，则阻止农田践踏
bypass-mob-griefing 
default: false
description: 为耕地设定为绕过暴虐的Gamerule
only-players-trample 
default: false
description: 如果只有玩家可以践踏农田，那就适用于真实。
disable-trampling 
default: false
description: 设置为true以完全禁用践踏。
feather-fall-distance-affects-trampling 
default: false
description: 如果实体可以停止践踏距离等于其羽毛水平的距离，则将其设置为True，加上首先践踏所需的额外块。羽毛1要求您跌落超过3个以上的街区以践踏。FF 2需要4+等。
spawner 
deactivate-by-redstone 
default: false
description: 允许由redstone停用的番茄岛
dispenser 
place-anvils 
default: false
description: 允许通过分配器放置砧座
anvil 
allow-colors 
Requires purpur.anvil.color permission
default: false
description: 允许玩家在砧座中使用颜色代码
cumulative-cost 
default: true
description: 如果在砧座中使用累积成本时应适用
lightning_rod 
range 
default: 128
description: 改变避雷针重定向闪电的范围
stonecutter 
damage 
default: 0.0
description:如果设置了一个值，则暴徒也将避免在斯托克官方上行走。
no-random-tick 
default: []
description: 不会随机勾选的块列表（仅适用于受随机勾选影响的块）
furnace 
use-lava-from-underneath 
default: false
description: 允许炉子由放置在它下面的熔岩无限制
blue_ice 
allow-snow-formation 
default: true
description: 设置为假，以禁止蓝冰上的冰层
chest 
open-with-solid-block-on-top 
default: false
description: 即使在顶部的固体块也允许箱子打开
shulker_box 
allow-oversized-stacks 
default: false
description: 控制是否允许在Shulker Boxes中允许过滤物品（默认修复块禁止发布Papermc / paper＃4748）
door 
requires-redstone 
default: []
description: 允许您设置需要redstone的门进行操作
twisting_vines 
growth-modifier 
default: 0.10
description: 改变藤蔓的增长率
max-growth-age 
default: 25
description: 植物可以生长的最大生长年龄
weeping_vines 
growth-modifier 
default: 0.10
description: 改变藤蔓的增长率
max-growth-age 
default: 25
description: The max growth age that the plant can grow
cave_vines 
growth-modifier 
default: 0.10
description: Changes the rate of growth of the vine
max-growth-age 
default: 25
description: 植物可以生长的最大生长年龄
powder_snow 
bypass-mob-griefing 
default: false
description: 为粉末雪设置为真实，以绕过暴民悲伤的gamerule
kelp 
max-growth-age 
default: 25
description: T植物可以生长的最大生长年龄
end-crystal 
baseless 
explode 
default: true
description: 设置为false以阻止晶体爆炸
explosion-power 
default: 6.0
description: 最终水晶爆炸的力量
explosion-fire 
default: false
description: Set to true to place fire when the end-crystal explodes
explosion-effect 
default: DESTROY
description: The type of explosion effect. Available values are NONE, BREAK, and DESTROY.
base 
explode 
default: true
description: Set to false to stop the crystal from exploding
explosion-power 
default: 6.0
description: The power of the end crystal's explosion
explosion-fire 
default: false
description: 当终端水晶爆炸时，设置为true以放置火灾
explosion-effect 
default: DESTROY
description: 爆炸效果的类型。可用值是没有，休息和销毁。
mobs 
ender_dragon 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description:让这个暴徒在水中掠夺（它不会弹出你）
ridable-max-y 
default: 256
description: 最大高度该暴徒可以在骑行时飞行
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
always-drop-full-exp 
default: false
description:当真正的所有有效的eNER龙死亡者都会降低全部经历球体，就像它是第一龙死亡一样
bypass-mob-griefing 
default: false
description: 设置为true，为reder dragon绕过暴民悲伤的gamerule
can-ride-vehicles 
default: false
description: 为reder dragon设置为true以获得骑车的能力
attributes 
max_health 
default: 200.0
description: Max Health属性
cave_spider 
ridable 
default: false
description:使这个暴徒是可控的
ridable-in-water 
default: false
description:让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 12.0
description: Max Health属性
endermite 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description:使这个暴徒在水中可铺展(it wont eject you)
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 8.0
description: Max health attribute
mooshroom 
ridable 
default: false
description: 使这个暴徒是可控的
rid
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 10.0
description: Max Health属性
polar_bear 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breedable-item 
default: ""
description: 诱惑/喂北极熊并使它们品种的物品
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 30.0
description: Max Health属性
vindicator 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description:让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
johnny 
spawn-chance 
default: 0.0
description: 百分比（0.0  -  1.0）名为“Johnny”的vindicator将产卵而不是vindicator
attributes 
max_health 
default: 24.0
description: Max Health属性
zombie_horse 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
spawn-chance 
default: 0.0
description: 百分比（0.0  -  1.0）一个僵尸马将产卵而不是骷髅马（在雷暴期间天然产卵）
attributes 
max_health 
min
default: 15.0
description: 最小健康属性
max
default: 15.0
description: Max Health属性
jump_strength 
min
default: 0.4
description: 最小jump_strength属性
max
default: 1.0
description: max jump_strength属性
movement_speed 
min
default: 0.2
description: MIN MOVION_SPEED属性
max
default: 0.2
description:最大moreformate_speed属性
wither 
ridable 
default: false
description:使这个暴徒是可控的
ridable-in-water 
default: false
description:让这个暴徒在水中掠夺（它不会弹出你）
ridable-max-y 
default: 256
description: 最大高度该暴徒可以在骑行时飞行
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
can-ride-vehicles 
default: false
description: 为枯萎设置骑行，以获得骑车的能力
play-spawn-sound 
default: true
description: 当它生成时，全球扮演枯萎的产卵声音
explosion-radius 
default: 1.0
description:枯萎的弹丸攻击的爆炸半径
health-regen-amount 
default: 1.0
description: 枯萎的制度金额
health-regen-delay 
default: 20
description: 延迟卫生的长度
bypass-mob-griefing 
default: false
description: 为枯萎绕过暴虐的Gamerule而定
attributes 
max_health 
default: 300.0
description:Max Health属性
wither_skeleton 
ridable 
default: false
description:使这个暴徒是可控的
ridable-in-water 
default: false
description: 使这个暴徒在水中可铺展(it wont eject you)
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 20.0
description: Max Health属性
zombie_villager 
ridable 
default: false
description:使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
cure 
enabled 
default: true
description: 设置为false以阻止僵尸村民可治愈
curing_time 
min 
default: 3600
description: 从固化时随机选择的最小蜱虫
max 
default: 6000
description: 从固化时随机选择的最大蜱量
jockey 
only-babies 
default: true
description:只有婴儿可以骑鸡
机会
default: 0.05
description: 产卵时骑鸡肉的百分比（0.0  -  1.0）
try-existing-chickens 
default: true
description: 扫描现有的鸡产卵
attributes 
max_health 
default: 20.0
description: Max Health属性
spawn_reinforcements 
default: 0.1
description:百分比（0.0  -  1.0）这个暴徒将产生增强
wandering_trader 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
can-be-leashed 
default: false
description: 允许玩家在村民身上使用潜在客户（交易者不包括）
allow-trading 
default: true
description: 设置为FALSE，以禁用Wandering Traders的交易
follow-emerald-blocks 
default: false
description: 村民们将被翡翠的街区诱惑，并关注持有它们的球员
attributes 
max_health 
default: 20.0
description: Max Health属性
silverfish 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
bypass-mob-griefing 
default: false
description: 设置为真正的银鱼来绕过暴徒悲伤的gamerule
attributes 
max_health 
default: 8.0
description: Max Health属性
zombified_piglin 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
count-as-player-kill-when-angry 
default: true
description: 如果他们被一名球员愤怒（但没有被杀），则将Zombized Piglins停止缩小XP
jockey 
only-babies 
default: true
description: 只有婴儿可以骑鸡
chance 
default: 0.05
description: 产卵时骑鸡肉的百分比（0.0  -  1.0）
try-existing-chickens 
default: true
description: 扫描现有的鸡产卵
attributes 
max_health 
default: 20.0
description: Max Health属性
spawn_reinforcements 
default: 0.0
description: 百分比（0.0  -  1.0）这个暴徒将产生增强
snow_golem 
用于确定镜头之间的蜱量的公式

((sqrt(distanceToTarget) / attack-distance) / snow-ball-modifier) * (max-shoot-interval-ticks - min-shoot-interval-ticks) + min-shoot-interval-ticks
If min-shoot-interval-ticks and max-shoot-interval-ticks are both set to 0, snow golems won't shoot any snowballs.
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 使这个暴徒在水中可铺展 (it wont eject you)
leave-trail-when-ridden 
default: false
description: 留下一条雪人在骑行时走的道路
drops-pumpkin-when-sheared 
default: true
description: 如果剪切雪人，则控制南瓜下降到地面
pumpkin-can-be-added-back 
default: false
description: 南瓜的控制可以放回雪人
min-shoot-interval-ticks 
default: 20
description: 最小的间隔蜱虫射击
max-shoot-interval-ticks 
default: 20
description: 获得拍摄的最大间隔刻度
snow-ball-modifier 
default: 10.0
description: 雪球射弹的改进剂价值
attack-distance 
default: 1.25
description:雪古博将攻击的距离
bypass-mob-griefing 
default: false
description: 为雪傀儡绕过暴徒悲伤的Gamerule设置为True
takes-damage-from-water 
default: true
description: 将此暴徒设置为FALSE，以停止损坏水
attributes 
max_health 
default: 4.0
description:Max Health属性
skeleton_horse 
can-swim 
default: false
description: 骨架马可以在水中游泳。假使它们沉入底部（vanilla默认）
ridable-in-water 
default: true
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
min
default: 15.0
description: 最小健康属性
max
default: 15.0
description: Max Health属性
jump_strength 
min
default: 0.4
description: 最小jump_strength属性
max
default: 1.0
description: max jump_strength属性
movement_speed 
min
default: 0.2
description: MIN MOVION_SPEED属性
max
default: 0.2
description: 最大moreformate_speed属性
phantom 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attacked-by-crystal-range 
default: 0.0
description: 半径晶体扫描幻影攻击。值0禁用功能
attacked-by-crystal-damage 
default: 1.0
description: 每秒晶体的损伤量对幻影交易。价值1.0是半心脏
orbit-crystal-radius 
default: 0.0
description: 半径的幻影扫描晶体到轨道。值0禁用功能
burn-in-light 
default: 0
description: 幽灵般的灯光会燃烧什么
burn-in-daylight 
default: true
description: 幽灵是在白天燃烧
flames-on-swoop 
default: false
description: 设置为真实的幻影击落俯冲的火焰
ignore-players-with-torch 
default: false
description: 幻影是否避免了手掌中带火炬的球员
allow-griefing 
default: false
description: 幻影的火焰是否可以燃烧物品
spawn 
min-sky-darkness 
default: 5
description: 天空中的黑暗量（5对雷暴足够暗，但不是定期雨）
only-above-sea-level 
default: true
description: 只产在海平面上方的球员上
only-with-visible-sky 
default: true
description: 只在他们上面有可见天空的球员上产卵
local-difficulty-chance 
default: 3.0
description: 本地难度必须大于0.0和此值之间选择的随机值
min-time-since-slept 
default: 72000
description: 自球员在产卵前睡觉以来的最小蜱次数
delay 
min
default: 1200
description: 产卵尝试（全球）之间的最短时间（在Ticks）
max
default: 2400
description: 产卵尝试（全球）之间的最长时间（在刻度）
overhead 
min
default: 20
description: 在球员头上产生的最小块数
max
default: 35
description: 在球员头上产生的最大块数
radius
default: 10
description:在球员头上产生的块半径
per-attempt 
min
default: 1
description: 每次尝试产生最小的幻影数量
max
default: -1
description: 每次尝试产生的最大幽灵数量（使用1以基于世界难度的基础）
attributes 
max_health 
default: 20.0
description: 最大的健康属性
chicken 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
retaliate 
default: false
description: 如果鸡被击中，它会攻击
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 4.0
description: Max Health属性
creeper 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
allow-griefing 
default: true
description: 设置为FALSE，以阻止爬行者悲伤。
bypass-mob-griefing 
default: false
description: 设置为true令爬行者绕过暴民悲伤的gamerule
naturally-charged-chance 
default: 0.0
description: 产卵时，百分比（0.0  -  1.0）爬行器（0.0  -  1.0）
explode-when-killed 
default: false
description: 在杀死时让爬行物爆炸
health-impacts-explosion 
default: false
description: 让爬行物的爆炸与它的卫生数量相称（较低的健康，较弱的爆炸）
attributes 
max_health 
default: 10.0
description: Max Health属性
donkey 
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
min
default: 15.0
description: 最小健康属性
max
default: 30.0
description: Max Health属性
jump_strength 
min
default: 0.5
description: 最小跳跃强度属性
max
default: 0.5
description: 最大跳跃强度属性
movement_speed 
min
default: 0.175
description: 最小运动速度属性
max
default: 0.175
description: 最大移动速度属性
cow 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
feed-mushrooms-for-mooshroom 
default: 0
description: 喂养牛的蘑菇数量使它变成摩源。值0禁用功能
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
naturally-aggressive-to-players 
chance 
default: 0.0
description: 百分比机会（0.0  -  1.0）这个暴徒将对玩家产生积极的攻击性
damage 
default: 2.0
description: 它将对玩家做的伤害金额
attributes 
max_health 
default: 10.0
description: Max Health属性
enderman 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
allow-griefing 
default: true
description: 设置为false以阻止恩德曼免受悲伤
can-despawn-with-held-block 
default: false
description: 即使它拿着一个街区，也让恩伯曼落花
ignore-projectiles 
default: false
description: 阻止恩德曼免受射弹
bypass-mob-griefing 
default: false
description: 为enderman设置为trup以绕过暴民悲伤的gamerule
takes-damage-from-water 
default: true
description: 将此暴徒设置为FALSE，以停止损坏水
aggressive-towards-endermites 
default: true
description: 设置为false，以阻止enderman争论争论所有类型的生成的邪恶
aggressive-towards-endermites-only-spawned-by-player-thrown-ender-pearls 
default: false
description: 只有当他们被抛出的珍珠队产卵时，才能让enderman agago才能使enderman aggro对邪教。这个选项没有任何权利侵略性 -  endermites是假的
ignore-players-wearing-dragon-head 
default: false
description: 设置为true让enderman忽略穿龙头的玩家
disable-player-stare-aggression 
default: false
description: 设置为true，以阻止一个望远镜眼睛的agdo agdo
attributes 
max_health 
default: 40.0
description: Max Health属性
evoker 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
bypass-mob-griefing 
default: false
description: 为牧师绕过暴民悲伤的Gamerule设置为true
attributes 
max_health 
default: 24.0
description: Max Health属性
drowned 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
can-break-doors 
default: false
description: 设置为true以允许淹死休息门
jockey 
only-babies 
default: true
description: 只有婴儿可以骑鸡
chance 
default: 0.05
description: 产卵时骑鸡肉的百分比（0.0  -  1.0）
try-existing-chickens 
default: true
description: 扫描现有的鸡产卵
attributes 
max_health 
default: 20.0
description: Max Health属性
spawn_reinforcements 
default: 0.1
description: 百分比（0.0  -  1.0）这个暴徒将产生增强
pillager 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
bypass-mob-griefing 
default: false
description: 设置为真正的枪手绕过暴徒悲伤的游戏
attributes 
max_health 
default: 24.0
description: Max Health属性
fox 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
tulips-change-type 
default: false
description: 喂白色/橙色郁金香改变类型雪/常规
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
bypass-mob-griefing 
default: false
description: 为狐狸设置为true绕过暴民悲伤的gamerule
attributes 
max_health 
default: 10.0
description: Max Health属性
giant 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
step-height 
default: 2.0
description: 不必跳跃有多少个块巨头可以走路
jump-height 
default: 1.0
description: 跳跃高度修饰符。默认值为1.0使巨头跳跃与腰部一样高
movement-speed 
default: 0.5
description: 运动速度属性
attack-damage 
default: 50.0
description: 攻击伤害（半心中）
have-ai 
default: false
description: 控制如果巨型僵尸有AI而不是站在那里
have-hostile-ai 
default: false
description: 如果巨型僵尸具有敌对的AI，则控制
attributes 
max_health 
default: 100.0
description: Max Health属性
hoglin 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 40.0
description: Max Health属性
glow_squid 
ridable 
default: false
description: 使这个暴徒是可控的
can-fly 
default: false
description: 让它如此鱿鱼可以飞，哦，我！
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 10.0
description: Max health attribute
squid 
ridable 
default: false
description: 使这个暴徒是可控的
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
immune-to-EAR 
default: true
description: 使这种暴徒免于耳朵（实体激活范围）
water-offset-check 
default: 0.0
description: 停止鱿鱼从水顶部漂浮
can-fly 
default: false
description: 让它如此鱿鱼可以飞，哦，我！
attributes 
max_health 
default: 10.0
description: Max Health属性
villager 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
brain-ticks 
default: 1
description: 村民蜱般的脑逻辑应该多久一次（在蜱虫中）。香草价值是打勾每一次刻度（1）。较高的量使它们不太经常勾选减少滞后，但将其设置得太高可能导致村民们没有响应村民
use-brain-ticks-only-when-lagging 
default: true
description: 当服务器滞后时，才能使用大脑刻度设置（参见上面的滞后阈值）。如果设置为false，则始终使用大脑刻度设置
bypass-mob-griefing 
default: false
description: 忽略了手动资产的Gamerule，让村民丢弃物品，让他们繁殖
can-be-leashed 
default: false
description: 允许玩家在村民身上使用潜在客户（交易者不包括）
follow-emerald-blocks 
default: false
description: 村民们将被翡翠的街区诱惑，并关注持有它们的球员
allow-trading 
default: true
description: 设置为FALSE以禁用与村民交易
can-breed 
default: true
description: 村民是否可以繁殖或不繁殖
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
clerics-farm-warts 
default: false
description: 为农民队的职员设置为真实
cleric-wart-farmers-throw-warts-at-villagers 
default: true
description: 为职员设置为False，不要在其他村民们扔幽灵疣
lobotomize 
enabled 
default: false
description: 如果不能移动（不禁用交易），请摇摇欲坠
check-interval 
default: 60
description: 蜱虫中的间隔检查村胎是否是leobotomized
spawn-iron-golem 
radius 
default: 0
description: Radius村民在产卵前搜索现有的铁傀儡。值0禁用功能
limit 
default: 0
description: 最大数量的铁傀儡村民可以在配置的半径中产生
attributes 
max_health 
default: 20.0
description: Max Health属性
mule 
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
min
default: 15.0
description: 最小健康属性
max
default: 30.0
description: Max Health属性
jump_strength 
min
default: 0.5
description: 最小跳跃强度属性
max
default: 0.5
description: 最大跳跃强度属性
movement_speed 
min
default: 0.175
description: 最小运动速度属性
max
default: 0.175
description: 最大移动速度属性
wolf 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
milk-cures-rabid-wolves 
default: true
description: 为rabid狼设置为false，不要被牛奶治愈
spawn-rabid-chance 
default: 0.0
description: 狼将作为rabid产卵的百分比（0.0  -  1.0）
default-collar-color 
default: RED
description: 何时命名狼时，请设置默认的套环颜色。可用颜色
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 8.0
description: Max Health属性
zoglin 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 40.0
description: Max Health属性
ocelot 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 10.0
description:Max Health属性
shulker 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
change-color-with-dye 
default: false
description: 通过用染料右键单击它来允许您更改Shulker的颜色
spawn-from-bullet: 
base-chance 
default: 1.0
description: 基础机会
require-open-lid 
default: true
description: 要求避难所让他们的盖子开放，从子弹产生
nearby-range 
default: 8.0
description: 附近的范围检查避难所
nearby-equation 
default: (nearby - 1) / 5.0
description: 用于计算从子弹施用的Shulker（附近是附近的Shulker实体的数量）的等式使得这是在附近有鲨的船只始终产卵
random-color 
default: false
description:  从Bulletset衍生时，突然涂上随机颜色
attributes 
max_health 
default: 30.0
description: Max Health属性
horse 
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
tempted-by-gold 
default: false
description: 在拿着金胡萝卜，金苹果或迷人的金苹果时，将这个暴徒设置为true。
stand-with-rider 
default: true
description: 如果一匹马（带骑车者）展示它的环境噪音
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
min
default: 15.0
description: 最小健康属性
max
default: 30.0
description: Max Health属性
jump_strength 
min
default: 0.4
description: 最小跳跃强度属性
max
default: 1.0
description: 最大跳跃强度属性
movement_speed 
min
default: 0.1125
description: 最小运动速度属性
max
default: 0.3375
description: 最大移动速度属性
piglin 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
bypass-mob-griefing 
default: false
description: 为猪圈设置为true以绕过暴虐的gamerule
portal-spawn-modifier 
default: 2000
description: 允许根据世界难度从门户块改变鸽子生成机会的修饰符。在这里阅读更多
attributes 
max_health 
default: 16.0
description: Max Health属性
piglin_brute 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 50.0
description: Max Health属性
skeleton 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 8.0
description: Max Health属性
stray 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 20.0
description: Max Health属性
goat 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 10.0
description: Max Health属性
panda 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 20.0
description: Max Health属性
strider 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
give-saddle-back 
default: false
description: 潜行并右键单击猪用马鞍，然后通过启用此选项将其删除
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
takes-damage-from-water 
default: true
description: 将此暴徒设置为FALSE，以停止损坏水
attributes 
max_health 
default: 20.0
description: Max Health属性
rabbit 
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
spawn-killer-rabbit-chance 
default: 0.0
description: 百分比（0.0-1.0）杀手兔自然产卵
spawn-toast-chance 
default: 0.0
description: 百分比（0.0-1.0）自然地产卵一只名叫多士的兔子
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
bypass-mob-griefing 
default: false
description: 设置为兔子绕过暴民悲伤的gamerule
attributes 
max_health 
default: 3.0
description: Max Health属性
husk 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
jockey 
only-babies 
default: true
description: 只有婴儿可以骑鸡
chance 
default: 0.05
description: 产卵时骑鸡肉的百分比（0.0  -  1.0）
try-existing-chickens 
default: true
description: 扫描现有的鸡产卵
attributes 
max_health 
default: 20.0
description: Max Health属性
spawn_reinforcements 
default: 0.1
description: 百分比（0.0  -  1.0）这个暴徒将产生增强
spider 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 16.0
description: Max Health属性
sheep 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
bypass-mob-griefing 
default: false
description: 为羊群绕过暴行悲伤的游戏乐曲
attributes 
max_health 
default: 8.0
description: Max Health属性
ravager 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
bypass-mob-griefing 
default: false
description: 设置为真正的拉瓦尔绕过暴徒悲伤的游戏
griefable-blocks 
default:

- minecraft:oak_leaves
- minecraft:spruce_leaves
- minecraft:birch_leaves
- minecraft:jungle_leaves
- minecraft:acacia_leaves
- minecraft:dark_oak_leaves
- minecraft:beetroots
- minecraft:carrots
- minecraft:potatoes
- minecraft:wheat
description: 可以被掠夺者打破的块白名单
attributes 
max_health 
default: 100.0
description: Max Health属性
pig 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
give-saddle-back 
default: false
description: 潜行并右键单击猪用马鞍，然后通过启用此选项将其删除
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 10.0
description: Max Health属性
witch 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 26.0
description: Max Health属性
zombie 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
jockey 
only-babies 
default: true
description: 只有婴儿可以骑鸡
chance 
default: 0.05
description: 产卵时骑鸡肉的百分比（0.0  -  1.0）
try-existing-chickens 
default: true
description: 扫描现有的鸡产卵
aggressive-towards-villager-when-lagging 
default: true
description: 禁止在滞后时阻止僵尸对村民的侵略性
bypass-mob-griefing 
default: false
description: 为僵尸绕过暴民悲伤的Gamerule设置为True
attributes 
max_health 
default: 20.0
description: Max health attribute
spawn_reinforcements 
default: 0.1
description: 百分比（0.0  -  1.0）这个暴徒将产生增强
dolphin 
ridable 
default: false
description: 使这个暴徒是可控的
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
naturally-aggressive-to-players-chance 
default: 0.0
description: 百分比机会（0.0  -  1.0）这个暴徒将对玩家产生积极的攻击性
disable-treasure-searching 
default: false
description: 从宝藏狩猎中停止海豚
spit 
cooldown 
default: 20
description: 海豚唾液的冷却时间
speed 
default: 1.0
description: 海豚唾液的速度
damage 
default: 2.0
description: 海豚吐的损害
attributes 
max_health 
default: 10.0
description: Max Health属性
axolotl 
ridable 
default: false
description: 使这个暴徒是可控的
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 14.0
description: Max Health属性
bat 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
ridable-max-y 
default: 256
description: 最大高度该暴徒可以在骑行时飞行
attributes 
max_health 
default: 6.0
description: Max Health属性
bee 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
ridable-max-y 
default: 256
description: 最大高度该暴徒可以在骑行时飞行
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
can-work-at-night 
default: false
description: 控制蜜蜂是否可以在夜间工作
can-work-in-rain 
default: false
description: 控制蜜蜂是否可以在多雨天气下工作
attributes 
max_health 
default: 10.0
description: Max Health属性
blaze 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
ridable-max-y 
default: 256
description: 最大高度该暴徒可以在骑行时飞行
takes-damage-from-water 
default: true
description: 将此暴徒设置为FALSE，以停止损坏水
attributes 
max_health 
default: 20.0
description: Max Health属性
cat 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
default-collar-color 
default: RED
description: 何时驯服CAT，请设置默认的套环颜色。可用颜色
spawn-delay 
default: 1200
description: 试图自然产生猫之间的蜱虫数
scan-range-for-other-cats 
swamp-hut 
default: 16
description: 如果在此范围内发现另一只猫，请不要产生一只猫。设置为0以禁用
village 
default: 48
description: Do not spawn a cat if another cat is found within this range. Set to 0 to disable
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 10.0
description: Max Health属性
cod 
ridable 
default: false
description: 使这个暴徒是可控的
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 3.0
description: Max Health属性
elder_guardian 
ridable 
default: false
description: 使这个暴徒是可控的
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 80.0
description: Max health attribute
ghast 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
ridable-max-y 
default: 256
description: 最大高度该暴徒可以在骑行时飞行
allow-griefing 
default: true
description: 设置为false以阻止Ghast悲伤
attributes 
max_health 
default: 10.0
description: Max Health属性
guardian 
ridable 
default: false
description: 使这个暴徒是可控的
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 30.0
description: Max Health属性
illusioner 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
naturally-spawn 
default: false
description: 如果幻觉者自然地在游戏中产生了控制
movement-speed 
default: 0.5
description: 运动速度属性
follow-range 
default: 18.0
description: 遵循范围属性
attributes 
max_health 
default: 32.0
description: Max Health属性
iron_golem 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
can-spawn-in-air 
default: false
description: 设置熨斗傀儡是否可以在空中产生，如1.12及以下
can-swim 
default: false
description: 设置熨斗狼群是否可以游泳
poppy-calms-anger 
default: false
description: 当它生气时，给烙铁古典将罂粟镇静下来
attributes 
max_health 
default: 100.0
description: Max Health属性
llama 
ridable 
default: false
description: 使这个暴徒是可控的。骆驼必须被驯服和背负（用地毯）是可控的。
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
tempted-by-hay 
default: false
description: 在拿着干草块时，将此暴徒设置为true
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
join-caravans 
default: true
description: 设置为false以禁用Llama Caravan功能
attributes 
max_health 
min
default: 15.0
description: 最小健康属性
max
default: 30.0
description: Max Health属性
jump_strength 
min
default: 0.5
description: 最小跳跃强度属性
max
default: 0.5
description: 最大跳跃强度属性
movement_speed 
min
default: 0.175
description: 最小运动速度属性
max
default: 0.175
description: 最大移动速度属性
trader_llama 
ridable 
default: false
description: 使该暴徒可安装和WASD可控。商人骆驼必须被驯服，以便是可控的。被鞍（地毯）并非如此，因为它在技术上总是有地毯。
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
min
default: 15.0
description: 最小健康属性
max
default: 30.0
description: Max Health属性
jump_strength 
min
default: 0.5
description: 最小跳跃强度属性
max
default: 0.5
description: 最大跳跃强度属性
movement_speed 
min
default: 0.175
description: 最小运动速度属性
max
default: 0.175
description: 最大移动速度属性
magma_cube 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: "size * size"
description: 用于计算最大健康的最大健康方程
parrot 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
ridable-max-y 
default: 256
description: 最大高度该暴徒可以在骑行时飞行
can-breed 
default: false
description: 给鹦鹉使用任何类型种子繁殖的能力（婴儿鹦鹉不存在D：，所以“成人”鹦鹉弹出）
attributes 
max_health 
default: 6.0
description: Max Health属性
pufferfish 
ridable 
default: false
description: 使这个暴徒是可控的
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 3.0
description: Max Health属性
salmon 
ridable 
default: false
description: Makes this mob WASD controllable
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 3.0
description: Max health attribute
slime 
ridable 
default: false
description: 使这个暴徒是可控的
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
attributes 
max_health 
default: "size * size"
description: 用于计算最大健康的最大健康方程
tropical_fish 
ridable 
default: false
description: 使这个暴徒是可控的
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
attributes 
max_health 
default: 3.0
description: Max Health属性
turtle 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
breeding-delay-ticks 
default: 6000
description: 在能够再次繁殖之前等待的蜱虫的数量
attributes 
max_health 
default: 30.0
description: Max Health属性
vex 
ridable 
default: false
description: 使这个暴徒是可控的
ridable-in-water 
default: false
description: 让这个暴徒在水中掠夺（它不会弹出你）
takes-damage-from-water 
default: false
description: 为这个暴徒设定为真的，开始从水中造成伤害
ridable-max-y 
default: 256
description: 最大高度该暴徒可以在骑行时飞行
attributes 
max_health 
default: 14.0
description: Max Health属性
gameplay-mechanics 
use-better-mending 
default: false
description: 设置为TRUE，用于修补魔法，以便首先修复最损坏的设备
mobs-ignore-rails 
default: false
description: 设置为true以允许小怪走过铁路
rain-stops-after-sleep 
default: true
description: 即使在球员睡觉之后，也可以让雨继续下去
thunder-stops-after-sleep 
default: true
description: 即使在球员睡觉之后，也会设置为FALSE
halloween 
force 
default: false
description: 设置为真实以迫使世界变成万圣节
head-chance 
default: 0.25
description: 百分比（0.0  -  1.0）僵尸或骨架将用杰克O'灯笼/雕刻南瓜在它的头上产生
mob-effects 
health-regen-amount 
default: 1.0
description: 此效果影响实体的金额
minimal-health-poison-amount 
default: 1.0
description: The amount at which this effect affects entities
poison-degeneration-amount 
default: 1.0
description: The amount at which this effect affects entities
wither-degeneration-amount 
default: 1.0
description: The amount at which this effect affects entities
hunger-exhaustion-amount 
default: 0.005
description: The amount at which this effect affects entities
saturation-regen-amount 
default: 1.0
description: 此效果影响实体的金额
projectiles-bypass-mob-griefing 
default: false
description: 设置为true for bultiles绕过暴民悲伤的gamerule
projectile-offset 
bow 
default: 1.0
description: 弓的射弹胶
crossbow 
default: 1.0
description: 弩的弹丸偏移
egg 
default: 1.0
description: 鸡蛋的弹丸偏移
ender-pearl 
default: 1.0
description: Ender-Pearl的弹丸偏移量
throwable-potion 
default: 1.0
description: 一个可口药水的射弹胶印
trident 
default: 1.0
description: 一个三叉戟的弹丸偏移
snowball 
default: 1.0
description: 雪球的弹丸偏移
drowning 
air-ticks 
default: 300
description: 在你开始溺水之前，你可以在水下呼吸多久
ticks-per-damage 
default: 20
description: 溺水伤害之间的蜱虫
damage-from-drowning 
default: 2.0
description: 溺水时完成的损害量
tick-fluids 
default: true
description: 设置为false以阻止流体滴答。使用此选项的简单插件的屏幕截图。附件：Freezefluids-1.0.jar
disable-drops-on-cramming-death 
default: false
description: 如果被挤满的gamerule杀死，请停止在死亡中删除战利品
entity-blindness-multiplier 
default: 1
description: 对盲目性药水效应的影响时，暴徒如何盲目
entities-pick-up-loot-bypass-mob-griefing 
default: false
description: 即使使手机的Gamerule被禁用，可以拿起战利品的怪物将继续拿起战利品
fix-climbing-bypassing-cramming-rule 
default: false
description: 通过攀登停止绕过填叫的游戏机的实体
milk-cures-bad-omen 
default: true
description:让玩家喝牛奶来治愈错误的预兆状态效果
trident-loyalty-void-return-height 
default: 0.0
description: 空隙高度，其中一个带有忠诚度的三叉戟将返回它的投掷者。值0.0或更高禁用此功能。
void-damage-dealt 
default: 4.0
description: 损坏的量损坏
void-damage-height 
default: -64.0
description: 空隙损坏的高度开始
entity-lifespan 
default: 0
description: 默认情况下禁用（0），滴答数实体将在消失之前生存。与玩家交互重置计时器
silk-touch 
需要purpur.drop.spawners和purpur.place.spawners权限

enabled 
default: false
description: 使它成为您可以使用带有丝绸触摸的工具的挖掘产卵器
minimal-level 
default: 1
description: 需要拿起矿产的丝绸触控水平的最小水平
tools 
default:

- minecraft:iron_pickaxe
- minecraft:golden_pickaxe
- minecraft:diamond_pickaxe
- minecraft:netherite_pickaxe
description: 可以用丝绸触摸挖掘产卵的工具白名单
spawner-name 
default: "<reset><white>Spawner"
description: spawner的名字
spawner-lore 
default:

- Spawns a <mob>
description: 水爪队的洛克
boat 
eject-players-on-land 
default: false
description: 船应该在陆地上弹出球员
do-fall-damage 
default: true
description: 为船只设置为FALSE，不要对玩家造成伤害
armorstand 
step-height 
default: 0.0
description: 设置Armorstands的默认步长高度。适用于使用Armorstands作为车辆的插件能够在不跳跃的情况下驾驶块，等等
set-name-visible-when-placing-with-custom-name 
default: false
description: 在使用自定义名称时使名称可见
fix-nametags 
default: false
description: 在装甲架上使用名称标签时使名称可见
place-with-arms-visible 
default: false
description: 让手臂放置时可见
can-movement-tick 
default: true
description: 设置为false以禁止搬运搬运
can-move-in-water 
default: true
description: 设置为FALSE，以禁止在水中移动的装甲
can-move-in-water-over-fence 
default: true
description: 设置为FALSE，以禁止装甲在围栏上移动水中
player 
shift-right-click-repairs-mending-points 
default: 0
description: 从玩家的酒吧使用的经验点数要修理在玩家库存中修复的物品
spawn-invulnerable-ticks 
default: 60
description: 在首次产卵时，可以控制玩家无法造成的长度才能控制的能力。
invulnerable-while-accepting-resource-pack 
default: false
description: 在下载资源包时将播放器设置为无懈可击。
teleport-if-outside-border 
default: false
description: 如果你以某种方式超出世界边境，那就传送你的产卵
totem-of-undying-works-in-inventory 
default: false
description: 允许在您的库存中运行不可见的图腾，而不仅仅是您的办公室
ridable-in-water 
default: false
description: 如果玩家在水中，让怪物/球员乘坐球员上
fix-stuck-in-portal 
default: false
description: 如果玩家在门户内被困在没有出门的门户内，步行到另一个块将重置门户电装机，允许它们通过门户网站传送返回
one-punch-in-creative 
default: false
description: 如果玩家在创意并用空的手击中实体，那么实体就会立即死亡
sleep-ignore-nearby-mobs 
default: false
description: 即使附近有暴徒，也可以允许睡眠
can-skip-night 
default: true
description: 设置为false禁用玩家通过睡觉跳过夜晚的能力
critical-damage-multiplier 
default: 1.5
description: 损害危害造成的百分比增加了基础损伤
burp-when-full 
default: false
description: 在玩家完全通过进食时填充饥饿吧后播放Burp声音
curse-of-binding 
remove-with-weakness 
default: false
description: 当它们具有应用于它们的弱点效果时，允许玩家去除绑定装甲的诅咒
armor-click-equip 
allow-hot-swapping 
default: false
description: 允许玩家通过右键单击在手中将盔甲交换在盔甲插槽中
creative-makes-copy 
default: true
description: 设置为FALSE，以便在右键单击将其放入播放器的盔甲插槽时，在手中重复装甲
idle-timeout 
kick-if-idle 
default: true
description: 踢球者如果他们变得空闲（请参阅播放器 - 空闲时间时间的服务器.Properties）
tick-nearby-entities 
default: true
description: 当附近的球员是AFK时，实体应该正常打勾。假将需要至少1名非AFK球员才能勾选
mobs-target 
default: true
description: 如果怪物瞄准附近的Afk球员
count-as-sleeping 
default: false
description: 如果afk玩家应该算作睡觉吗？（允许活跃的玩家通过睡觉跳过夜晚，即使Afk球员不在床上）
update-tab-list 
default: false
description: 如果AFK播放器在选项卡列表中更新了他们的名称（在他们的名字前面放在其中[AFK]）
exp-dropped-on-death 
equation 
default: expLevel * 7
description: 降低了多少exp。可用的NMS变量是Explevel，Exptotal和Exp
maximum 
default: 100
description: 降低死亡的最大exp值金额
netherite-fire-resistance 
duration 
default: 0
description: 设定耐火性持续时间。设置为0以禁用
amplifier 
default: 0
description: 将放大器设置为防火效应
ambient 
default: false
description: 设置为true以使粒子效果在屏幕上更少侵入
show-particles 
default: false
description: 设定为真实的防火药水效应显示颗粒
show-icon 
default: true
description: 设置为FALSE对于防火效应，不显示它的图标
minecart 
max-speed 
default: 0.4
description: 受控时Minecart的最大速度
place-anywhere 
default: false
description: 是否可以在任何地方放置minecarts，而不仅仅是在轨道上
powered-rail 
boost-modifier 
default: 0.06
description: Minecarts获得从击中动力轨道的速度提升（不会影响炉子Minecarts）
controllable 
enabled 
default: false
description: 如果不在轨道上时可以控制minecarts
fall-damage 
default: true
description: 设置为true以在minecart时对播放器造成损坏
step-height 
default: 1.0
description: Minecarts可以在不跳转的情况下延长下一个块的阶梯高度
hop-boost 
default: 0.5
description: 按下可控的Minecart上的空格键时跳跃电源
base-speed 
default: 0.1
description: 受控时Minecart的基本速度
block-speed 
default:

grass_block: 0.3
stone: 0.5
description: 每个块类型的速度覆盖列表
item 
shears 
damage-if-sprinting 
default: false
description: 冲刺时持有剪切将随机损坏玩家（不要用剪刀运行！）
sprinting-damage 
default: 1
description: 启用损坏 -  Sprinting是否启用了损坏的损坏量
snowball 
extinguish 
fire 
default: false
description: 雪球是否抛出时，应该熄灭火灾
candles 
default: false
description: 扔雪球，什么时候应该熄灭蜡烛
campfires 
default: false
description: 滚雪球是否抛出时，应该熄灭篝火
shulker_box 
drop-contents-when-destroyed 
default: true
description: 当Shulker盒子被摧毁时是否应该丢弃它的内容
compass 
holding-shows-bossbar 
default: false
description: 如果来自/罗盘命令的Bossbar应该在拿着指南针时显示
glow_berries 
eat-glow-duration 
default: 0
description: 蜱虫在吃漂亮的浆果后，玩家会发出的蜱。设置为0以禁用
ender-pearl 
damage 
default: 5
description: 使用eAder珍珠传送后损坏的损害量
cooldown 
default: 20
description: 使用Ender Pearl后的冷却时间（在蜱虫中）
creative-cooldown 
default: 20
description: 在创意时使用eAder珍珠后的冷却时间（在蜱虫中）
endermite-spawn-chance 
default: 0.05
description: 百分比（0.0-1.0）endermite将在使用eAder珍珠传送之后产卵
immune 
explosion 
default: []
description: 免疫爆炸的物品清单
fire 
default: []
description: 清单免受火灾的物品
lightning 
default: []
description: 免于闪电的物品清单
cactus 
default: []
description: 免疫仙人掌的物品清单
Example of item immune list:

explosion:
  - minecraft:diamond
  - minecraft:diamond_block
  - minecraft:diamond_sword
Warning
这些物品免疫列表可能导致客户端desync问题，例如地面上的看不见物品！从服务器端代码中没有任何内容可以完成。

elytra 
damage-per-second 
default: 1
description: Elytra在每秒飞行期间造成了多少伤害
damage-multiplied-by-speed 
default: 0.0
description: 如果飞行比设定速度快，则损坏乘以速度。值0禁用此乘法器
kinetic-damage 
default: true
description: 球员在飞入墙壁时应该受到伤害
ignore-unbreaking 
default: false
description: Elytras应该忽略未破坏的魅力
damage-per-boost 
firework 
default: 0
description: 烟花升压激活时对Elytra造成损害多少
trident 
default: 0
description: 当三叉戟旋转升压激活时，对Elytra交易的损害是多少
mob-spawning 
village-cats 
default: default
description: 在世界上塑造成真的，这个选项是其中的一部分
raid-patrols 
default: default
description: Set to true to spawn in the world that this option is a part of
phantoms 
default: default
description: Set to true to spawn in the world that this option is a part of
wandering-traders 
default: default
description: Set to true to spawn in the world that this option is a part of
village-sieges 
default: default
description: 在世界上塑造成真的，这个选项是其中的一部分
raid-cooldown-seconds 
default: 0
description: 您应该在另一个RAID之前等待多长时间
projectile-despawn-rates 
dragon_fireball 
default: -1
description: 滴定滴定在蜱虫中的速度。-1意味着残疾人
egg 
default: -1
description: The rate at which the projectile despawns in ticks. -1 means disabled
ender_pearl 
default: -1
description: The rate at which the projectile despawns in ticks. -1 means disabled
experience_bottle 
default: -1
description: The rate at which the projectile despawns in ticks. -1 means disabled
firework_rocket 
default: -1
description: The rate at which the projectile despawns in ticks. -1 means disabled
fishing_bobber 
default: -1
description: The rate at which the projectile despawns in ticks. -1 means disabled
fireball 
default: -1
description: The rate at which the projectile despawns in ticks. -1 means disabled
llama_spit 
default: -1
description: The rate at which the projectile despawns in ticks. -1 means disabled
potion 
default: -1
description: The rate at which the projectile despawns in ticks. -1 means disabled
shulker_bullet 
default: -1
description: The rate at which the projectile despawns in ticks. -1 means disabled
small_fireball 
default: -1
description: The rate at which the projectile despawns in ticks. -1 means disabled
snowball 
default: -1
description: 滴定滴定在蜱虫中的速度。-1
means disabled
wither_skull 
default: -1
description: 滴定滴定在蜱虫中的速度。-1意味着残疾人
entities-can-use-portals 
default: true
description: 设置为false以停止实体能够使用门户
persistent-tileentity-display-names-and-lore 
default: false
description: 设置为true以使TE的显示名称和LOROR在分手后持续存在（例如，命名的自定义播放器头保留他们的名字）
persistent-droppable-entity-display-names 
default: false
description: 设置为true以使实体的显示姓名和LOROR在断开后持续存在（例如名为ARMOR Stands保留他们的名字）
infinity-bow 
normal-arrows 
default: true
description: 设置为true以使Infinity enchantment在此箭头类型上工作
spectral-arrows 
default: false
description: 设置为true以使Infinity enchantment在此箭头类型上工作
tipped-arrows 
default: false
description: 设置为true以使Infinity enchantment在此箭头类型上工作
works-without-arrows 
default: false
description: 设置为真实的无限蝴蝶，没有箭头
daylight-cycle-ticks 
daytime 
default: 12000
description: 设置季节循环的截留时间
nighttime 
default: 12000
description: 设置夜间周期被勾选多长时间
animal-breeding-cooldown-seconds 
default: 0
description: 每只动物类型增加一个繁殖动物
projectile-damage 
snowball 
default: -1
description: 设置雪球的损坏程度（-1将为违约实体为燃烧者造成3个损坏3，默认情况下）
entity-left-handed-chance 
default: 0.05
description: 百分比（0.0  -  1.0）实体将左撇子产生
fireballs-bypass-mob-griefing 
default: false
description: 设置为Fireballs以绕过暴虐的Gamerule
note-block-ignore-above 
default: false
description: 设置为true for note块以继续发出声音，即使它上面有一个块
impose-teleport-restrictions-on-gateways 
default: false
description: 设置为true以在网关上施加传送限制。这将广播entitytelepterndinderedEvent事件，如果由于乘客/是车辆，如果他们失败，则可以重试传送的能力
always-tame-in-creative 
default: false
description: 设置为true，有100％的机会驯服暴徒
shovel-turns-block-to-grass-path 
default:

- minecraft:coarse_dirt
- minecraft:dirt
- minecraft:grass_block
- minecraft:mycelium
- minecraft:podzol
- minecraft:rooted_dirt
description: 右键单击铲子时可以变成草图的块列表
ridable-settings 
babies-are-ridable 
default: true
description: 设置为false以阻止婴儿被可取
untamed-tamables-are-ridable 
default: true
description: 设置为false以停止无法获得的可恶可行
use-night-vision 
default: false
description: 设置为true，让夜视给骑士的骑行