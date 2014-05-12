<?xml version="1.0"?>
<map proto="1.3.2">
<name>Decline</name>
<version>1.3.0</version>
<objective>Destory the other team's 2 Orb monuments to win!</objective>
<authors>
  <author>minimitch0199</author>
</authors>
<contributors>
  <contributor contribution="Helping out with buildings">ParaSpider</contributor>
  <contributor contribution="XML Help">Captain_Elliott</contributor>
</contributors>
<rules>
  <rule>Fall damage is disabled!</rule>
</rules>
<teams>
  <team color="orange" max="35" max-overfill="50">Orange Team</team>
  <team color="dark purple" max="35" max-overfill="50">Purple Team</team>
</teams>
<kits>
  <!-- Only given to Observers -->
  <kit name="default" force="false">
    <potion duration="oo" amplifier="4">NIGHT_VISION</potion>
  </kit>
  <kit name="spawn-effects" force="false">
    <potion duration="10" amplifier="10">REGENERATION</potion>
    <potion duration="10" amplifier="10">DAMAGE_RESISTANCE</potion>
    <potion duration="oo" amplifier="2">SPEED</potion>
  </kit>
  <kit name="spawn" parents="spawn-effects">
    <item slot="0" name="`3Sword `7[Tier 0]" attributes="generic.attackDamage:add:2">wood sword</item>
    <item slot="8" amount="1" name="`3Shard of Twilight">nether quartz</item>
  </kit>
  <kit name="orange" parents="spawn">
    <helmet color="d87f33" name="`3Helmet `7[Tier 0]">leather helmet</helmet>
    <chestplate color="d87f33" name="`3Chestplate `7[Tier 0]">leather chestplate</chestplate>
  </kit>
  <kit name="purple" parents="spawn">
    <helmet color="7f3fb2" name="`3Helmet `7[Tier 0]">leather helmet</helmet>
    <chestplate color="7f3fb2" name="`3Chestplate `7[Tier 0]">leather chestplate</chestplate>
  </kit>
</kits>
<spawns>
  <default kit="default" yaw="135">
    <cuboid min="16,59,12" max="16,59,12"/>
  </default>
  <spawn team="orange" kit="orange" yaw="180">
    <cuboid min="81,43,4" max="84,43,5"/>
  </spawn>
  <spawn team="purple" kit="purple" yaw="0">
    <cuboid min="22,43,269" max="25,43,270"/>
  </spawn>
</spawns>
<destroyables materials="ice;glass;lapis block;emerald block" completion="100%">
  <destroyables owner="orange">
    <destroyable name="Front Monument">
      <cuboid min="75,32,61" max="69,40,55"/>
    </destroyable>
    <destroyable name="Back Monument">
      <cuboid min="19,29,40" max="13,37,34"/>
    </destroyable>
  </destroyables>
  <destoryables owner="purple">
    <destroyable name="Front Monument">
      <cuboid min="31,32,213" max="37,40,219"/>
    </destroyable>
    <destroyable name="Back Monument">
      <cuboid min="87,29,234" max="93,37,240"/>
    </destroyable>
  </destoryables>
</destroyables>
<blockdrops>
  <rule>
    <region>
      <cuboid min="-oo,oo,-oo" max="oo,oo,oo"/>
    </region>
    <filter>
      <block>glass</block>
    </filter>
    <drops>
      <item amount="1" name="`3Shard of Twilight">nether quartz</item>
    </drops>
    <experience>0</experience>
    <replacement>air</replacement>
    <wrongtool>true</wrongtool>
  </rule>
</blockdrops>
<filters>
  <filter name="deny-water">
    <deny>
      <any>
        <block>water</block>
        <block>stationary water</block>
      </any>
    </deny>
  </filter>
  <filter name="allow-tnt" parents="deny-blocks">
    <allow>
      <block>tnt</block>
    </allow>
  </filter>
  <filter name="only-orange" parents="deny-players">
    <allow>
      <team>orange</team>
    </allow>
  </filter>
  <filter name="only-purple" parents="deny-players">
    <allow>
      <team>purple</team>
    </allow>
  </filter>
  <filter name="deny-blocks" parents="deny-blocks"/>
  <filter name="breakables" parents="deny-blocks">
    <allow>
      <block>diamond ore</block>
    </allow>
  </filter>
</filters>
<!-- Regions and Proximities -->
<toolrepair>
  <tool>wood sword</tool>
  <tool>stone sword</tool>
  <tool>iron sword</tool>
  <tool>diamond sword</tool>
  <tool>leather helmet</tool>
  <tool>leather chestplate</tool>
  <tool>leather leggings</tool>
  <tool>chainmail chestplate</tool>
  <tool>chainmail leggings</tool>
  <tool>iron chestplate</tool>
  <tool>iron leggings</tool>
  <tool>bow</tool>
</toolrepair>
<itemremove>
  <item>wood sword</item>
  <item>stone sword</item>
  <item>iron sword</item>
  <item>diamond sword</item>
  <item>leather helmet</item>
  <item>leather chestplate</item>
  <item>leather leggings</item>
  <item>chain chestplate</item>
  <item>chain leggings</item>
  <item>iron chestplate</item>
  <item>iron leggings</item>
  <item>arrow</item>
  <item>tnt</item>
  <item>blaze rod</item>
  <item>stone pickaxe</item>
  <item>glass bottle</item>
  <item>potion</item>
  <item>diamond</item>
  <item>redstone torch</item>
  <item>spruce log</item>
  <item>stone bricks</item>
  <item>stone brick stairs</item>
  <item>stone brick slab</item>
  <item>ladder</item>
  <item>spruce wood</item>
  <item>spruce wood stairs</item>
  <item>spruce wood slab</item>
  <item>sign</item>
  <item>jungle sapling</item>
  <item>seeds</item>
</itemremove>
<itemkeep>
  <item>diamond chestplate</item>
  <item>gold helmet</item>
  <item>gold sword</item>
  <item>bow</item>
<mobs>
  <filter>
    <spawn>spawner</spawn>
  </filter>
</mobs>
<modifybowprojectile>
  <projectile>FireBall</projectile>
  <velocityMod>2.5</velocityMod>
  <potion duration="6" amplifier="1">BLINDNESS</potion>
</modifybowprojectile>
<disabledamage>
  <!-- Disable fall damage -->
  <damage>fall</damage>
  <!-- TNT damages enemies and self, but not teammates -->
  <damage ally="true" self="false" enemy="false" other="false">block explosion</damage>
</disabledamage>
<tnt>
  <instantignite>on</instantignite>
  <blockdamage>on</blockdamage>
  <yield>0</yield>
</tnt>
<killreward>
  <item amount="2" name="`3Shard of Twilight">nether quartz</item>
</killreward>
<gamerules>
  <doDaylightCycle>false</doDaylightCycle>
</gamerules>
<hunger>
  <depletion>off</depletion>
</hunger>
<multitrade/>
<include src="tutorial.xml"/>
<tutorial>
  <stage title="Decline">
    <message>
      <line>
        `rThis map is a `a`lDTM/Gear `rmap.
      </line>
      <line>
        The objective is to destroy the other team's two monuments.
      </line>
    </message>
  </stage>
  <stage title="Monuments">
    <message>
      <line>
        `rThis is one of the two `a`lMonuments `ryou have to defend.
      </line>
      <line>
        `rDestroying the other teams monuments will not only help your team, but will reward you.
      </line>
      <line>
        `rFor every glass block broken, you will be rewared with a `3`lShard of Twilight`r.
      </line>
    </message>
    <teleport>
      <point yaw="-130" pitch="40">64,41,64</point>
    </teleport>
  </stage>
  <stage title="The Archmage">
    <message>
      <line>
        `rThis is the home of the `5Twilight Archmage `rand her minions `6Fate `rand `cGlory`r. They hit quite hard, so be careful!
      </line>
      <line>
        `rThe `5Twilight Archmage `rwill drop a `5Twilight Gemstone `rwhen killed. While `6Fate `rwill drop a `6Dust of Fate `r and `cGlory `rwill drop a `cDust for Glory`r.
      </line>
      <line>
        `rThese items can be used to buy higher tiered gear.
      </line>
    </message>
    <teleport>
      <point yaw="-45" pitch="15">81,39,107</point>
    </teleport>
  </stage>
  <stage title="Home Teleporters">
    <message>
      <line>
        `rThese towers will teleport you back to your spawn tower when ever you need to get back!
      </line>
      <line>
        `rYou need to be careful, because the enemy can come along and `cdestroy `rthe tower so you can't use it.
      </line>
    </message>
  </stage>
</tutorial>
</map>
