Minecraft-Crash
===============

Minecraft Crash
---- Minecraft Crash Report ----
// Who set us up the TNT?

Time: 05/01/13 15:34
Description: Failed to start game

cpw.mods.fml.common.LoaderException: java.lang.NoSuchMethodError: forestry.api.genetics.IAlleleRegistry.getRegisteredBranches()Ljava/util/LinkedHashMap;
  at cpw.mods.fml.common.LoadController.transition(LoadController.java:117)
	at cpw.mods.fml.common.Loader.initializeMods(Loader.java:660)
	at cpw.mods.fml.client.FMLClientHandler.finishMinecraftLoading(FMLClientHandler.java:207)
	at net.minecraft.client.Minecraft.a(Minecraft.java:456)
	at asq.a(SourceFile:56)
	at net.minecraft.client.Minecraft.run(Minecraft.java:744)
	at java.lang.Thread.run(Unknown Source)
Caused by: java.lang.NoSuchMethodError: forestry.api.genetics.IAlleleRegistry.getRegisteredBranches()Ljava/util/LinkedHashMap;
	at binnie.core.genetics.BreedingSystem.calculateArrays(BreedingSystem.java:86)
	at binnie.core.BinnieCore.postInit(BinnieCore.java:64)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at cpw.mods.fml.common.FMLModContainer.handleModStateEvent(FMLModContainer.java:483)
	at sun.reflect.GeneratedMethodAccessor3.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at com.google.common.eventbus.EventHandler.handleEvent(EventHandler.java:69)
	at com.google.common.eventbus.SynchronizedEventHandler.handleEvent(SynchronizedEventHandler.java:45)
	at com.google.common.eventbus.EventBus.dispatch(EventBus.java:317)
	at com.google.common.eventbus.EventBus.dispatchQueuedEvents(EventBus.java:300)
	at com.google.common.eventbus.EventBus.post(EventBus.java:268)
	at cpw.mods.fml.common.LoadController.propogateStateMessage(LoadController.java:140)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at com.google.common.eventbus.EventHandler.handleEvent(EventHandler.java:69)
	at com.google.common.eventbus.SynchronizedEventHandler.handleEvent(SynchronizedEventHandler.java:45)
	at com.google.common.eventbus.EventBus.dispatch(EventBus.java:317)
	at com.google.common.eventbus.EventBus.dispatchQueuedEvents(EventBus.java:300)
	at com.google.common.eventbus.EventBus.post(EventBus.java:268)
	at cpw.mods.fml.common.LoadController.distributeStateMessage(LoadController.java:83)
	at cpw.mods.fml.common.Loader.initializeMods(Loader.java:659)
	... 5 more


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- System Details --
Details:
	Minecraft Version: 1.4.6
	Operating System: Windows 8 (amd64) version 6.2
	Java Version: 1.7.0_10, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 108987192 bytes (103 MB) / 259653632 bytes (247 MB) up to 2649489408 bytes (2526 MB)
	LiteLoader Mods: 3 loaded mod(s)
          - VoxelPacket version 2.0.1
          - VoxelPlayer version 0.9.3
          - VoxelMenu version 1.4.6
	JVM Flags: 5 total; -Xms256M -Xmx2560M -XX:+UseConcMarkSweepGC -XX:+CMSIncrementalMode -XX:+AggressiveOpts
	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	Suspicious classes: FML and Forge are installed
	IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
	FML: MCP v7.25 FML v4.6.17.515 Minecraft Forge 6.5.0.489 Feed The Beast Mod Pack 73 mods loaded, 73 mods active
	mcp [Minecraft Coder Pack] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	FML [Forge Mod Loader] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	Forge [Minecraft Forge] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	mod_CodeChickenCore [CodeChicken Core] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	mod_NotEnoughItems [Not Enough Items] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	denLib [denLib] (denLib-2.1.4.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	BuildCraft|Core [BuildCraft] (buildcraft-A-3.3.0.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	BuildCraft|Energy [BC Energy] (buildcraft-A-3.3.0.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	ExtrabiomesXL [ExtrabiomesXL] (ExtrabiomesXL-universal-1.4.6-3.7.0.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	Forestry [Forestry for Minecraft] (forestry-A-1.7.0.1.jar) Unloaded->Constructed->Pre-initialized->Initialized->Errored
	IC2 [IndustrialCraft 2] (industrialcraft-2_1.112.170-lf.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	drceph.petrogen [Petroleum Generator] ([1.4.6]PetroGen-1.1.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	mod_ReiMinimap [mod_ReiMinimap] ([1.4.6]ReiMinimap_v3.2_06.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	AdvancedMachines [IC2 Advanced Machines Addon] (AdvancedMachines_4.7a.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	BuildCraft|Builders [BC Builders] (buildcraft-A-3.3.0.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	BuildCraft|Factory [BC Factory] (buildcraft-A-3.3.0.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	BuildCraft|Transport [BC Transport] (buildcraft-A-3.3.0.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	BuildCraft|Silicon [BC Silicon] (buildcraft-A-3.3.0.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	ValvePipe [Valve Pipe] (BuildCraft-Z-ValvePipeAM-1.4.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	ChickenChunks [ChickenChunks] (ChickenChunks 1.2.1.1.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	ComputerCraft [ComputerCraft] (ComputerCraft1.481.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	CCTurtle [ComputerCraft Turtles] (ComputerCraft1.481.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	EnderStorage [EnderStorage] (EnderStorage 1.3.1.1.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	BinnieCore [Binnie Core] (extrabees-1.4.9.6-prerelease.zip) Unloaded->Constructed->Pre-initialized->Initialized->Errored
	ExtraBees [Extra Bees] (extrabees-1.4.9.6-prerelease.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	factorization [Factorization] (Factorization-0.7.10.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	Railcraft [Railcraft] (Railcraft_1.4.6-6.13.1.0.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	RedPowerCore [RedPower] (RedPowerCore-2.0pr6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	RedPowerBase [RP Base] (RedPowerCore-2.0pr6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	RedPowerMachine [RP Machine] (RedPowerMechanical-2.0pr6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	RedPowerCompat [RP Compat] (RedPowerCompat-2.0pr6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	RedPowerWiring [RP Wiring] (RedPowerDigital-2.0pr6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	RedPowerLogic [RP Logic] (RedPowerDigital-2.0pr6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	RedPowerLighting [RP Lighting] (RedPowerDigital-2.0pr6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	RedPowerWorld [RP World] (RedPowerMechanical-2.0pr6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	RedPowerControl [RP Control] (RedPowerMechanical-2.0pr6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	ThermalExpansion [Thermal Expansion] (ThermalExpansion-2.1.6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	ThermalExpansion|Factory [Factory] (ThermalExpansion-2.1.6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	ThermalExpansion|Energy [Energy] (ThermalExpansion-2.1.6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	ThermalExpansion|Transport [Transport] (ThermalExpansion-2.1.6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	TwilightForest [The Twilight Forest] (twilightforest-1.14.0.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	XyCraft [XyCraft] (xycraft-universal-1.4.6-0.9.44.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	GregTech_Addon [GregTech-Addon] (GregTechMod_2.73c.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	IC2NuclearControl [Nuclear Control] (IC2NuclearControl-1.4.5.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	mod_InvTweaks [Inventory Tweaks] (InventoryTweaks_1.46.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	IronChest [Iron Chest] (ironchest-universal-1.4.6-4.5.1.203.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	MiscPeripherals [MiscPeripherals] (miscperipherals-2.3.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	AdvancedSolarPanel [Advanced Solar Panels] (mod_AdvancedSolarPanels_3_3_2.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	GraviSuite [Gravitation Suite] (mod_zGraviSuite_1_6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	ModularForceFieldSystem [Modular ForceField System V2] (ModularForceFieldSystemV2.2.8.2.14.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	Mystcraft [Mystcraft] (mystcraft-uni-1.4.6-0.9.5.00.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	NEIPlugins [NEI Plugins] (NEIPlugins-1.0.4.1.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	ObsidiPlates [Obsidian Pressure Plates] (obsidiplates-universal-1.2.0.3.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	OmniTools [OmniTools] (OmniTools-2.2.5.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	LiquidRoundup [Liquid Roundup] (PluginsforForestry2-Complete-Build20.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	PluginsforForestry|Core [PluginsforForestry|Core] (PluginsforForestry2-Complete-Build20.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	PluginsforForestry|BlueFood [PluginsforForestry|BlueFood] (PluginsforForestry2-Complete-Build20.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	PluginsforForestry|BuildCraft [PluginsforForestry|BuildCraft] (PluginsforForestry2-Complete-Build20.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	PluginsforForestry|Forestry [PluginsforForestry|Forestry] (PluginsforForestry2-Complete-Build20.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	PluginsforForestry|Ic2 [PluginsforForestry|Ic2] (PluginsforForestry2-Complete-Build20.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	PluginsforForestry|Railcraft [PluginsforForestry|Railcraft] (PluginsforForestry2-Complete-Build20.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	PluginsforForestry|RedPower2 [PluginsforForestry|RedPower2] (PluginsforForestry2-Complete-Build20.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	Thaumcraft [Thaumcraft] (Thaumcraft3.0.1c.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	PluginsforForestry|Thaumcraft [PluginsforForestry|Thaumcraft] (PluginsforForestry2-Complete-Build20.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	PluginsforForestry|Tweaks [PluginsforForestry|Tweaks] (PluginsforForestry2-Complete-Build20.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	PortalGun [Portal Gun] (portalgun1.4.6v2.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	SoulShards [SoulShards] (SoulShards-v1.21-universal.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	StevesCarts [Steve's Carts] (StevesCarts2.0.0.a41.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	ThermalExpansion|NEI [NEI] (ThermalExpansion-NEI-2.1.6.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	TC [Traincraft] (Traincraft-3.1.13_010.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	WR-CBE|Core [WR-CBE Core] (WR-CBE Core 1.3.2.4.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	WR-CBE|Addons [WR-CBE Addons] (WR-CBE Addons 1.3.2.4.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	WR-CBE|RedPower [WR-CBE RedPower] (WR-CBE RedPower 1.3.2.4.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized
	LWJGL: 2.4.2
	OpenGL: GeForce GT 640/PCIe/SSE2 GL version 4.2.0, NVIDIA Corporation
	Is Modded: Definitely; Client brand changed to 'forge,fml'
	Type: Client (map_client.txt)
	Texture Pack: Default
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: ~~ERROR~~ NullPointerException: null
