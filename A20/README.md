# A20

## 效果说明

### 寒冷抗性

<passive_effect name="HypothermalResist" operation="base_add" value="100"/>

### 炎热抗性

<passive_effect name="HyperthermalResist" operation="base_add" value="100"/>

### 力量

<passive_effect name="AttributeLevel" tags="attStrength" operation="base_add" value="10"/>

### 感知

<passive_effect name="AttributeLevel" tags="attPerception" operation="base_add" value="10"/>

### 强健

<passive_effect name="AttributeLevel" tags="attFortitude" operation="base_add" value="10"/>

### 敏捷

<passive_effect name="AttributeLevel" tags="attAgility" operation="base_add" value="10"/>

### 智慧

<passive_effect name="AttributeLevel" tags="attIntellect" operation="base_add" value="10"/>

### 交易

<passive_effect name="BarteringBuying" operation="base_add" value="1"/>
<passive_effect name="BarteringSelling" operation="base_add" value="1"/>

### 制作时间

<passive_effect name="CraftingTime" operation="perc_add" value="-1"/>

### 经验值

<passive_effect name="PlayerExpGain" operation="perc_add" value="10"/>

### 行走速度

<passive_effect name="WalkSpeed" operation="base_set" value="2"/>
<passive_effect name="WalkSpeed" operation="perc_add" value="4"/>


### 跑步速度

<passive_effect name="RunSpeed" operation="base_set" value="4"/>
<passive_effect name="RunSpeed" operation="perc_add" value="6"/>

### 体力消耗

<passive_effect name="StaminaChangeOT" operation="perc_add" value="1" tags="walking"/>
<passive_effect name="StaminaChangeOT" operation="perc_add" value="1" tags="running"/>

### 物理防御

<passive_effect name="PhysicalDamageResist" operation="base_add" value="1000"/>
<passive_effect name="PhysicalDamageResist" operation="base_add" value="10,100" tier="1,6"/>

### 辐射防御

<passive_effect name="ElementalDamageResist" operation="base_add" value="1000" tags="heat,electrical"/>
<passive_effect name="ElementalDamageResist" operation="base_add" value="10,100" tier="1,6"/>

### 装备耐久

<passive_effect name="DegradationMax" operation="base_set" value="1000,6000" tier="1,6"/>
<passive_effect name="DegradationPerUse" operation="base_set" value="0" tags="heavyArmorDeg"/>

### 噪音

<passive_effect name="NoiseMultiplier" operation="perc_add" value="-1"/>

## 装备名称（item name）

作战服上装
apparelArmyShirt

作战服下装
apparelArmyPants

雪茄 力量+1 交易+10%
apparelCigar

墨镜 感知+1
apparelShades

硬汉墨镜 强健+1
apparelToughGuySunglasses

滑雪护目镜 敏捷+1
apparelSkiGoggles

书虫眼镜 智慧+1 制作时间-10% 获得经验值+10%
apparelNerdGlasses

吉利服套装
apparelGhillieSuitHood
apparelGhillieSuitJacket
apparelGhillieSuitPants

钢套装
armorSteelHelmet
armorSteelChest
armorSteelGloves
armorSteelLegs
armorSteelBoots

军用套装
armorMilitaryHelmet
armorMilitaryVest
armorMilitaryGloves
armorMilitaryLegs
armorMilitaryBoots
armorMilitaryStealthBoots

砍刀
meleeWpnBladeT3Machete

手枪
gunHandgunT1Pistol

猎枪
gunRifleT3SniperRifle

塔萨的石斧
meleeToolRepairT0TazasStoneAxe

岩石克星
buffDrugRockBusters

.44沙漠秃鹰传奇组合包
questRewardT3HandgunLegendaryBundle

生存大礼包
questRewardT3SurvivalLegendaryBundle

木框架
woodShapes

基岩
terrBedrock

安全木门
secureDoorWooden

<item name="questRewardT3SurvivalLegendaryBundle">
	<property name="Extends" value="noteTestersDelightAdmin"/>
	<property name="CreativeMode" value="Player"/>
	<property name="CustomIcon" value="bundlePistol"/>
	<property name="CustomIconTint" value="FFFFFF"/>
	<property name="ItemTypeIcon" value="bundle"/>
	<property name="DescriptionKey" value="questRewardLegendaryRangedWeaponBundleDesc"/>
	<property class="Action0">
		<property name="Create_item" value="meleeToolRepairT0TazasStoneAxe,gunHandgunT1Pistol,ammo9mmBulletBall,modDyePink,apparelGhillieSuitJacket,apparelGhillieSuitPants,armorMilitaryHelmet,modArmorHelmetLight"/>
		<property name="Create_item_count" value="6,6,300,3,1,1,6,1"/>
	</property>
</item>

<item name="gunHandgunT1Pistol">
	<property name="Tags" value="weapon,ranged,holdBreathAiming,reloadPenalty,gun,shortRange,pistol,barrelAttachments,sideAttachments,smallTopAttachments,magazine,firingMode,attAgility,perkGunslinger,9mmGun,attachmentsIncluded,canHaveCosmetic"/>
	<property name="DisplayType" value="rangedGun"/>
	<property name="HoldType" value="1"/>
	<property name="Meshfile" value="#Other/Items?Weapons/Ranged/Pistol/PistolPrefab.prefab"/>
	<property name="Material" value="MHandGunParts"/> <property name="Weight" value="4"/>
	<property name="RepairTools" value="resourceRepairKit"/>
	<property name="DegradationBreaksAfter" value="false"/>
	<property name="SoundJammed" value="weapon_jam"/>
	<property name="Attachments" value="meleeToolFlashlight02"/>
	<property name="CrosshairOnAim" value="true"/> <!-- aimTest -->
	<property name="CrosshairUpAfterShot" value="true"/> <!-- aimTest -->
	<property name="Sound_Sight_In" value="pistol_sight_in"/>
	<property name="Sound_Sight_Out" value="pistol_sight_out"/>
	<property name="LightSource" value="lightSource"/> <!-- Start: Needed for the attachment flashlight -->
	<property name="ActivateObject" value="Attachments/flashlight/lightSource"/>
	<property name="AttachmentFlashlight" value="flashlight02"/> <!-- End: Needed for the attachment flashlight -->
	<property name="Group" value="Ammo/Weapons,Ranged Weapons"/>
	<property name="RepairExpMultiplier" value="10.8"/>
	<property name="LightValue" value=".45"/>
	<property name="EconomicValue" value="500"/>
	<property name="UnlockedBy" value="perkGunslinger,gunHandgunT1PistolSchematic"/>
    <property name="ShowQuality" value="true"/>

	<property class="Action0">
		<property name="Class" value="Ranged"/>
		<property name="Magazine_items" value="ammo9mmBulletBall,ammo9mmBulletHP,ammo9mmBulletAP"/>
		<property name="Sound_start" value="Pistol_Fire"/>
		<property name="Sound_loop" value="Pistol_Fire"/>
		<property name="Sound_end" value=""/>
		<property name="Sound_empty" value="dryfire"/>
		<property name="Sound_reload" value="pistol_reload"/>
		<property name="AutoReload" value="false"/>
		<property name="Particles_muzzle_fire" value="gunfire_pistol"/>
		<property name="Particles_muzzle_fire_fpv" value="gunfire_pistol_fpv"/>
		<requirement name="CVarCompare" cvar="_underwater" operation="LT" value=".98"/>
	</property>
	<property class="Action1">
		<property name="Class" value="Zoom"/>
		<property name="Zoom_max_out" value="55"/>
		<property name="Zoom_max_in" value="55"/>
		<property name="ScopeCameraOffset" value="0,.0008,0"/>
	</property>

	<effect_group name="gunHandgunT1Pistol">
		<passive_effect name="MaxRange" operation="base_set" value="999" tags="perkGunslinger,9mmGun"/>
		<passive_effect name="DamageFalloffRange" operation="base_set" value="999" tags="perkGunslinger,9mmGun"/>
		<passive_effect name="DamageFalloffRange" operation="perc_add" value="-.2,.2" tags="perkGunslinger,9mmGun"/> <!-- random effective rng -->

		<passive_effect name="RoundsPerMinute" operation="base_set" value="180" tags="perkGunslinger"/>
		<passive_effect name="BurstRoundCount" operation="base_set" value="1" tags="perkGunslinger"/>
		<passive_effect name="ReloadSpeedMultiplier" operation="base_set" value="10" tags="perkGunslinger"/> <!-- 2.7s -->

		<passive_effect name="MagazineSize" operation="base_set" value="99" tags="perkGunslinger"/>
		 <!--<passive_effect name="ReloadSpeedMultiplier" operation="base_set" value="1" tags="perkGunslinger"/> 2s -->
		<passive_effect name="ModSlots" operation="base_set" value="1,1,2,2,3,4" tier="1,2,3,4,5,6"/>
		<passive_effect name="ModPowerBonus" operation="perc_add" value=".10" tags="EntityDamage,BlockDamage"/>
		<passive_effect name="ModPowerBonus" operation="base_add" value="300" tags="EconomicValue"/>

		<passive_effect name="EntityDamage" operation="perc_add" value="999" tags="perkGunslinger"/> <!-- random EntityDmg -->
		<passive_effect name="EntityDamage" operation="perc_add" value="999" tier="2,6" tags="perkGunslinger"/> <!-- tier bonus -->
		<passive_effect name="BlockDamage" operation="perc_add" value="0" tags="perkGunslinger"/> <!-- random BlockDmg -->
		<passive_effect name="BlockDamage" operation="perc_add" value="0" tier="2,6" tags="perkGunslinger"/> <!-- tier bonus -->

		<passive_effect name="DegradationMax" operation="perc_add" value="-.2,.2" tags="perkGunslinger"/> <!-- random DegMax -->
		<passive_effect name="RoundsPerMinute" operation="perc_add" value="-.05,.05" tags="perkGunslinger"/> <!-- random APM -->
		<passive_effect name="MagazineSize" operation="perc_add" value="-.122,.122"/> <!-- random MagazineSize -->
		<passive_effect name="WeaponHandling" operation="perc_add" value="-.08,.08" tags="perkGunslinger"/> <!-- random WeaponHandling -->

		<passive_effect name="SpreadDegreesVertical" operation="base_set" value="1.5" tags="perkGunslinger"/>
		<passive_effect name="SpreadDegreesHorizontal" operation="base_set" value="1.5" tags="perkGunslinger"/>
		<passive_effect name="SpreadMultiplierAiming" operation="base_set" value=".4" tags="perkGunslinger"/>
		<passive_effect name="SpreadMultiplierCrouching" operation="base_set" value=".8" tags="perkGunslinger"/>
		<passive_effect name="SpreadMultiplierWalking" operation="base_set" value="1.5" tags="perkGunslinger"/>
		<passive_effect name="SpreadMultiplierRunning" operation="base_set" value="2.2" tags="perkGunslinger"/>

		<passive_effect name="KickDegreesVerticalMin" operation="base_set" value=".7" tags="perkGunslinger"/>
		<passive_effect name="KickDegreesVerticalMax" operation="base_set" value=".8" tags="perkGunslinger"/>
		<passive_effect name="KickDegreesHorizontalMin" operation="base_set" value="-.25" tags="perkGunslinger"/>
		<passive_effect name="KickDegreesHorizontalMax" operation="base_set" value=".25" tags="perkGunslinger"/>

		<passive_effect name="IncrementalSpreadMultiplier" operation="base_set" value="2.0" tags="perkGunslinger,9mmGun"/>
		<passive_effect name="WeaponHandling" operation="base_set" value=".95" tags="perkGunslinger"/> <!-- crosshair reset speed -->

		<passive_effect name="DegradationMax" operation="base_set" value="250,999" tier="1,6" tags="perkGunslinger,9mmGun"/>
		<passive_effect name="DegradationPerUse" operation="base_set" value="0" tags="perkGunslinger,9mmGun"/>
	</effect_group>
</item>

<item name="meleeToolRepairT0TazasStoneAxe">
	<property name="Extends" value="meleeToolRepairT0StoneAxe"/>
	<property name="Tags" value="axe,melee,light,tool,longShaft,tazas,repairTool,miningTool,attStrength,perkMiner69r,perkMotherLode,perkTheHuntsman,canHaveCosmetic"/>
	<property name="EconomicValue" value="1000"/>
	<property name="CustomIcon" value="meleeToolRepairT0StoneAxe"/> <property name="CustomIconTint" value="ffb0b0"/>
	<property class="Action0">
		<!-- <property name="Stamina_usage" value="4.5"/> DEPRECATED stat -->
	</property>
	<property class="Action1"> <!-- UseAction -->
		<property name="Class" value="Repair"/>
		<property name="Delay" value=".5"/> <!-- Repair actions still need the delay amount -->
		<property name="Repair_amount" value="5000"/>
		<property name="Upgrade_hit_offset" value="-5"/>
		<property name="Sound_start" value="repair_block"/>
		<property name="Allowed_upgrade_items" value="resourceWood,resourceClayLump,resourceSnowBall,resourceScrapIron,resourceForgedIron,resourceForgedSteel,resourceConcreteMix,resourceCobblestones,ironDoor1_v1,vaultDoor01,scrapHatch_v1,vaultHatch_v1,cellarDoorDoubleIron,cellarDoorDoubleSteel,shuttersIronBlockVariantHelper,shuttersSteelBlockVariantHelper,resourceYuccaFibers,resourceCloth,resourceScrapPolymers"/>
		<property name="UsePowerAttackAnimation" value="false"/>
	</property>
	<effect_group name="meleeToolRepairT0TazasStoneAxe">
		<!-- This item gets a free pass on random stats because it's not craftable. -->
		<passive_effect name="EntityDamage" operation="base_set" value="999" tags="perkMiner69r"/>
		<passive_effect name="BlockDamage" operation="base_set" value="999" tags="perkMiner69r"/>
		<passive_effect name="AttacksPerMinute" operation="base_set" value="105" tags="perkMiner69r,axe"/>
		<passive_effect name="StaminaLoss" operation="base_set" value="-10" tags="primary"/>
		<passive_effect name="DegradationMax" operation="base_set" value="120,999" tier="1,6" tags="perkMiner69r"/>
		<passive_effect name="DegradationPerUse" operation="base_set" value="0" tags="perkMiner69r"/>
		<passive_effect name="MaxRange" operation="base_set" value="999" tags="perkMiner69r"/>
		<passive_effect name="BlockRange" operation="base_set" value="999" tags="perkMiner69r"/>

		<passive_effect name="ModSlots" operation="base_set" value="1,1,2,2,3,4" tier="1,2,3,4,5,6"/>
		<passive_effect name="ModPowerBonus" operation="perc_add" value=".10" tags="EntityDamage,BlockDamage"/>
		<passive_effect name="ModPowerBonus" operation="base_add" value="300" tags="EconomicValue"/>

		<passive_effect name="EntityDamage" operation="perc_add" value="999" tags="perkMiner69r"/> <!-- random EntityDmg -->
		<passive_effect name="EntityDamage" operation="perc_add" value="999" tier="2,6" tags="perkMiner69r"/> <!-- tier bonus -->
		<passive_effect name="BlockDamage" operation="perc_add" value="999" tags="perkMiner69r"/> <!-- random BlockDmg -->
		<passive_effect name="BlockDamage" operation="perc_add" value="999" tier="2,6" tags="perkMiner69r"/> <!-- tier bonus -->
		<passive_effect name="DegradationMax" operation="perc_add" value="1" tags="perkMiner69r"/> <!-- random DegMax -->
		<passive_effect name="AttacksPerMinute" operation="perc_add" value="-.05,.05" tags="perkMiner69r"/> <!-- random APM -->
		<passive_effect name="StaminaLoss" operation="perc_add" value="-1"/> <!-- random StamLoss -->

		<display_value name="dBlockRepairAmount" value="100"/>
		<passive_effect name="HarvestCount" operation="base_set" value="10" tags="butcherHarvest"/>
		<passive_effect name="HarvestCount" operation="perc_add" value="10" tags="oreWoodHarvest"/>
		<passive_effect name="DamageModifier" operation="perc_add" value="-.85" tags="earth"/>
		<passive_effect name="DamageModifier" operation="perc_add" value="-.33" tags="stone"/>
		<passive_effect name="DamageModifier" operation="perc_add" value="-.5" tags="metal"/>
	</effect_group>
</item>

<item name="apparelGhillieSuitJacket">
	<property name="Extends" value="apparelPlantFiberMaster" param1="CustomIcon"/>
	<property name="UnlockedBy" value="perkSniperComplete"/>
	<property name="Tags" value="chest,clothing,pocketMod,canHaveCosmetic"/>
	<property name="EquipSlot" value="Chest"/>
	<property name="DisplayType" value="clothingGhillie"/>
	<property name="DescriptionKey" value="apparelGhillieSuitGroupDesc"/>
	<property class="UMA">
		<property name="Mesh" value="ghillie_suit_shirt"/>
		<property name="Overlay0" value="ghillie_suit"/>
		<property name="Overlay0Tint" value="105,110,83"/>
		<property name="Layer" value="3"/>
		<property name="UISlot" value="Jacket"/>
		<property name="Mask0" value="hands" param1="outer"/>
		<property name="Mask1" value="chest" param1="middle"/>
	</property>
	<effect_group tiered="false">
		<passive_effect name="ModSlots" operation="base_set" value="1"/>
		<passive_effect name="ModPowerBonus" operation="base_add" value="100" tags="EconomicValue"/>
		<passive_effect name="HypothermalResist" operation="base_add" value="100"/>
		<passive_effect name="HyperthermalResist" operation="base_add" value="100"/>
		<passive_effect name="LightMultiplier" operation="perc_add" value="-1"><requirement name="!IsIndoors"/></passive_effect>
		<passive_effect name="LightMultiplier" operation="perc_add" value="-1"><requirement name="IsIndoors"/></passive_effect>
		<display_value name="dLightMultiplier" value="-1"/>
		<passive_effect name="NoiseMultiplier" operation="perc_add" value="-1"/><display_value name="dNoiseMultiplier" value="-1"/>
		<passive_effect name="AttributeLevel" tags="attStrength" operation="base_add" value="10"/>
		<passive_effect name="AttributeLevel" tags="attPerception" operation="base_add" value="10"/>
		<passive_effect name="AttributeLevel" tags="attFortitude" operation="base_add" value="10"/>
		<passive_effect name="AttributeLevel" tags="attAgility" operation="base_add" value="10"/>
		<passive_effect name="AttributeLevel" tags="attIntellect" operation="base_add" value="10"/>
		<passive_effect name="BarteringBuying" operation="base_add" value="1"/>
		<passive_effect name="BarteringSelling" operation="base_add" value="1"/>
		<passive_effect name="CraftingTime" operation="perc_add" value="-1"/>
		<passive_effect name="PlayerExpGain" operation="perc_add" value="10"/>
		<passive_effect name="WalkSpeed" operation="base_set" value="2"/>
		<passive_effect name="RunSpeed" operation="base_set" value="5"/>
		<passive_effect name="StaminaChangeOT" operation="perc_add" value="1" tags="walking"/>
		<passive_effect name="StaminaChangeOT" operation="perc_add" value="1" tags="running"/>
	</effect_group>
</item>

<item name="apparelGhillieSuitPants">
	<property name="Extends" value="apparelPlantFiberMaster" param1="CustomIcon"/>
	<property name="UnlockedBy" value="perkSniperComplete"/>
	<property name="Tags" value="legs,clothing,pocketMod,canHaveCosmetic"/> <!-- clothing = dyeable -->
	<property name="EquipSlot" value="Legs"/>
	<property name="DisplayType" value="clothingGhillie"/>
	<property name="DescriptionKey" value="apparelGhillieSuitGroupDesc"/>
	<property class="UMA">
		<property name="Mesh" value="ghillie_suit_pants"/>
		<property name="Overlay0" value="ghillie_suit"/>
		<property name="Overlay0Tint" value="105,110,83"/>
		<property name="Layer" value="1"/>
		<property name="UISlot" value="Pants"/>
	</property>
	<effect_group tiered="false">
		<passive_effect name="ModSlots" operation="base_set" value="1"/>
		<passive_effect name="ModPowerBonus" operation="base_add" value="100" tags="EconomicValue"/>
		<passive_effect name="HypothermalResist" operation="base_add" value="100"/>
		<passive_effect name="HyperthermalResist" operation="base_add" value="100"/>
		<passive_effect name="LightMultiplier" operation="perc_add" value="-1"><requirement name="!IsIndoors"/></passive_effect>
		<passive_effect name="LightMultiplier" operation="perc_add" value="-1"><requirement name="IsIndoors"/></passive_effect>
		<display_value name="dLightMultiplier" value="-1"/>
		<passive_effect name="NoiseMultiplier" operation="perc_add" value="-1"/><display_value name="dNoiseMultiplier" value="-1"/>
	</effect_group>
</item>

<item name="armorMilitaryHelmet">
	<property name="Extends" value="armorMilitaryMaster" param1="CustomIcon"/>
	<property name="Tags" value="head,armor,armorHead,lightArmor,lightArmorPenalty,canHaveCosmetic,lightArmorDeg"/>
	<property name="EquipSlot" value="Head"/>
	<effect_group name="military armor">
		<passive_effect name="ModSlots" operation="base_set" value="1,1,2,2,3,4" tier="1,2,3,4,5,6"/>
		<passive_effect name="ModPowerBonus" operation="base_add" value="300" tags="EconomicValue"/>
		<passive_effect name="PhysicalDamageResist" operation="base_add" value="9999"/>
		<passive_effect name="PhysicalDamageResist" operation="base_add" value="999" tier="1,6"/>
		<passive_effect name="ElementalDamageResist" operation="base_add" value="9999" tags="heat,electrical"/>
		<passive_effect name="ElementalDamageResist" operation="base_add" value="999" tier="1,6"/>
		<passive_effect name="BuffResistance" operation="base_add" value="9999" tags="buffFatiguedTrigger,buffArmSprainedCHTrigger,buffLegSprainedCHTrigger,buffLaceration,buffInfectionCatch,buffInjuryStunned01CHTrigger,buffInjuryBleedingTwo,buffInjuryBleedingBarbedWire,critResistDisplay"/>
		<passive_effect name="DegradationMax" operation="base_set" value="9999" tier="1,6"/>
		<passive_effect name="DegradationPerUse" operation="base_set" value="0" tags="lightArmorDeg"/>
		<passive_effect name="Mobility" operation="perc_add" value="1"/>
		<passive_effect name="StaminaChangeOT" operation="perc_add" value="-.0281" tags="walking"/>
		<passive_effect name="StaminaChangeOT" operation="perc_add" value="-.0562" tags="running"/>
		<display_value name="dStaminaChangeOT" value="-.56"/>
		<passive_effect name="NoiseMultiplier" operation="perc_add" value=".1"/><display_value name="dNoiseMultiplier" value=".1"/>
	</effect_group>
	<property class="UMA">
		<property name="Mesh" value="gear_kevlar_helmet"/>
		<property name="Overlay0" value="gear_kevlar_helmet"/>
		<property name="Layer" value="2"/>
		<property name="UISlot" value="Headgear"/>
		<property name="ShowAltHair" value="true"/>
	</property>
</item>

questRewardT3SurvivalLegendaryBundle,items,item,,,666,,666,666,666,666,666,666,666,666,666,666,生存大礼包,666,666

name="DifficultyTier" value="5"
