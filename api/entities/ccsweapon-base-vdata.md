## ccsweapon_base_vdata

此类型表示武器的静态数据。

## built_right_handed

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示武器是否为右手设计。

## allow_flipping

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示武器是否可以翻转为左手使用。

## linked_cooldowns

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示武器的冷却时间是否与其他武器关联。

## flags

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

表示与武器相关的各种标志。

## primary_ammo_type

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

主弹夹使用的弹药类型。

## secondary_ammo_type

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

副弹夹使用的弹药类型。

## max_clip1

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

主弹夹可容纳的最大子弹数。

## max_clip2

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

副弹夹可容纳的最大子弹数。

## default_clip1

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

主弹夹的默认子弹数。

## default_clip2

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

副弹夹的默认子弹数。

## reserve_ammo_as_clips

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示备用弹药是否以额外弹夹的形式存储。

## weight

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

表示武器的重量。

## auto_switch_to

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示拾取时游戏是否会自动切换到此武器。

## auto_switch_from

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示游戏是否会自动从此武器切换到其他武器。

## rumble_effect

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

表示与此武器相关的震动效果。

## slot

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

此武器占用的库存槽位。

## position

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

武器在库存槽位中的位置。

## weapon_type

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`csweapon_type`](/api/entities/csweapon-type "此枚举表示游戏中的武器类型。")

武器的类型。

## weapon_category

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`csweapon_category`](/api/entities/csweapon-category "此枚举表示游戏中武器的分类。")

武器的分类。

## gear_slot

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

表示与武器相关的装备槽位。

## gear_slot_position

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

武器在装备槽位中的位置。

## default_loadout_slot

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

武器的默认装备槽位。

## s_wrong_team_msg

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `string`

当错误的队伍使用武器时显示的消息。

## price

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

武器的购买价格。

## kill_award

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

使用此武器击杀后给予玩家的现金奖励。

## primary_reserve_ammo_max

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

主弹夹的最大备用弹药量。

## secondary_reserve_ammo_max

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

副弹夹的最大备用弹药量。

## melee_weapon

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示武器是否被归类为近战武器。

## has_burst_mode

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示武器是否具有连发模式。

## is_revolver

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示武器是否被归类为左轮手枪。

## cannot_shoot_underwater

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示武器是否不能在水下射击。

## name

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `string`

武器的内部名称。

## anim_extension

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `string`

武器使用的动画扩展名。

## e_silencer_type

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

表示与武器兼容的消音器类型。

## crosshair_min_distance

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

此武器的最小准星扩散距离。

## crosshair_delta_distance

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

射击时准星扩散距离的变化。

## is_full_auto

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示武器是否为全自动。

## num_bullets

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

每次射击发射的子弹数量。

## cycle_time

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

连续射击之间的时间间隔。

## max_speed

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

持有此武器时玩家的最大移动速度。

## spread

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

武器射击时的基础扩散。

## inaccuracy_crouch

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

武器在蹲下时的不准确性。

## inaccuracy_stand

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

武器在站立时的不准确性。

## inaccuracy_jump

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

武器在跳跃时的不准确性。

## inaccuracy_land

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

武器在从跳跃落地时的不准确性。

## inaccuracy_ladder

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

武器在攀爬梯子时的不准确性。

## inaccuracy_fire

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

武器在射击时的不准确性。

## inaccuracy_move

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

武器在移动时的不准确性。

## recoil_angle

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

武器射击时的后座角度。

## recoil_angle_variance

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

后座角度变化的方差。

## recoil_magnitude

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

武器射击时的后座幅度。

## recoil_magnitude_variance

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<float>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

后座幅度变化的方差。

## tracer_frequency

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`cfiring_mode<int>`](/api/entities/ccsweapon-base-vdata/cfiring-mode "射击模式信息。")

射击武器时可见的弹壳频率。

## inaccuracy_jump_initial

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器在跳跃时的初始不准确性。

## inaccuracy_jump_apex

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器在跳跃顶点的不准确性。

## inaccuracy_reload

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器在重新加载后的不准确性。

## recoil_seed

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

用于确定后座模式的模式种子值。

## spread_seed

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

用于确定武器扩散的模式种子值。

## time_to_idle_after_fire

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器在射击后过渡到空闲的时间。

## idle_interval

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器空闲动画之间的间隔时间。

## attack_movespeed_factor

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

使用此武器攻击时玩家移动速度减少的比例。

## heat_per_shot

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器每射击产生的热量。

## inaccuracy_pitch_shift

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

射击不准确性引起的音高变化。

## inaccuracy_alt_sound_threshold

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

不准确性达到何种程度时播放替代声音的阈值。

## bot_audible_range

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

机器人可以听到此武器射击的范围。

## use_radio_subtitle

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `string`

表示此武器是否使用无线电字幕来执行其操作。

## unzooms_after_shot

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示武器是否会在射击后自动缩放。

## hide_view_model_when_zoomed

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `bool`

表示当武器缩放时是否隐藏视图模型。

## zoom_levels

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

此武器可用的缩放级别数量。

## zoom_fov1

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

第一个缩放级别的视野（FOV）。

## zoom_fov2

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

第二个缩放级别的视野（FOV）。

## zoom_time0

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

过渡到初始缩放状态的时间。

## zoom_time1

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

过渡到第一个缩放级别的时间。

## zoom_time2

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

过渡到第二个缩放级别的时间。

## iron_sight_pull_up_speed

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器铁瞄拉起速度。

## iron_sight_put_down_speed

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器铁瞄放下速度。

## iron_sight_fov

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器铁瞄在瞄准武器铁瞄时的视野（FOV）。

## iron_sight_pivot_forward

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器铁瞄的前枢轴点。

## iron_sight_looseness

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器铁瞄在瞄准时的松动性。

## ang_pivot_angle

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`vector`](/api/common-types/vector "此类型是常见的3D向量（x, y, z）。")

武器铁瞄的枢轴角度。

## vec_iron_sight_eye_pos

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`vector`](/api/common-types/vector "此类型是常见的3D向量（x, y, z）。")

武器铁瞄在瞄准时的眼睛位置。

## damage

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

武器的基础伤害。

## headshot_multiplier

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

应用于头部射击的伤害倍增器。

## armor_ratio

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

确定伤害穿透装甲的比例。

## penetration

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器对材料的穿透能力。

## range

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

武器的有效射程。

## range_modifier

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

应用于基于范围的伤害修饰符。

## flinch_velocity_modifier_large

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

大挫败效果的速度修饰符。

## flinch_velocity_modifier_small

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

小挫败效果的速度修饰符。

## recovery_time_crouch

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

在蹲下时恢复准确性的时间。

## recovery_time_stand

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

站立时恢复准确性的时间。

## recovery_time_crouch_final

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

在蹲下时最终恢复准确性的时间。

## recovery_time_stand_final

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

站立时最终恢复准确性的时间。

## recovery_transition_start_bullet

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

恢复过渡开始的子弹数量。

## recovery_transition_end_bullet

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `int`

恢复过渡结束的子弹数量。

## throw_velocity

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `float`

抛出物品（例如，手榴弹）的速度。

## v_smoke_color

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: [`vector`](/api/common-types/vector "此类型是常见的3D向量（x, y, z）。")

此武器的烟雾效果颜色。

## anim_class

[![Field][此字段是一个普通字段，必须使用点(.)来访问]rw]
[![Read Only][此字段是只读字段，你不能更改其值。这不适用于子字段（如果有的话）]r]

类型: `string`

与该武器关联的动画类。