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
