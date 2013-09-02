---- Minecraft Crash Report ----
// Quite honestly, I wouldn't worry myself about that.

Time: 13-9-2 19:45
Description: Unexpected error

java.lang.IllegalStateException: Already tesselating!
	at bfn.b(Tessellator.java:480)
	at bfi.a(RenderGlobal.java:1851)
	at bfi.a(RenderGlobal.java:1836)
	at bfb.a(EntityRenderer.java:1613)
	at bfb.b(EntityRenderer.java:1115)
	at ats.S(SourceFile:686)
	at ats.d(SourceFile:619)
	at net.minecraft.client.main.Main.main(SourceFile:101)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at bfn.b(Tessellator.java:480)
	at bfi.a(RenderGlobal.java:1851)
	at bfi.a(RenderGlobal.java:1836)
	at bfb.a(EntityRenderer.java:1613)

-- Affected level --
Details:
	Level name: MpServer
	All players: 2 total; [bdf['minile6as'/257619, l='MpServer', x=-92,94, y=66,62, z=329,54], bev['ImVeXii'/207080, l='MpServer', x=-17,31, y=65,00, z=305,47]]
	Chunk stats: MultiplayerChunkCache: 441
	Level seed: 0
	Level generator: ID 00 - default, ver 1. Features enabled: false
	Level generator options: 
	Level spawn location: World: (2366,11,-2620), Chunk: (at 14,0,4 in 147,-164; contains blocks 2352,0,-2624 to 2367,255,-2609), Region: (4,-6; contains chunks 128,-192 to 159,-161, blocks 2048,0,-3072 to 2559,255,-2561)
	Level time: 16815229 game time, 17742586 day time
	Level dimension: 0
	Level storage version: 0x00000 - Unknown?
	Level weather: Rain time: 0 (now: false), thunder time: 0 (now: false)
	Level game mode: Game mode: survival (ID 0). Hardcore: false. Cheats: false
	Forced entities: 52 total; [bdf['minile6as'/257619, l='MpServer', x=-92,94, y=66,62, z=329,54], bev['ImVeXii'/207080, l='MpServer', x=-17,31, y=65,00, z=305,47], tv['Zombie'/249682, l='MpServer', x=-15,31, y=65,00, z=305,69], bev['ImVeXii'/207080, l='MpServer', x=-17,31, y=65,00, z=305,47], tv['Zombie'/249690, l='MpServer', x=-15,31, y=65,00, z=305,69], oc['entity.ItemFrame.name'/804, l='MpServer', x=-218,50, y=66,50, z=324,94], oc['entity.ItemFrame.name'/805, l='MpServer', x=-220,50, y=66,50, z=324,94], oc['entity.ItemFrame.name'/806, l='MpServer', x=-222,50, y=66,50, z=324,94], oc['entity.ItemFrame.name'/800, l='MpServer', x=-210,50, y=66,50, z=324,94], oc['entity.ItemFrame.name'/801, l='MpServer', x=-212,50, y=66,50, z=324,94], oc['entity.ItemFrame.name'/802, l='MpServer', x=-214,50, y=66,50, z=324,94], oc['entity.ItemFrame.name'/803, l='MpServer', x=-216,50, y=66,50, z=324,94], sr['item.item.rottenFlesh'/229948, l='MpServer', x=-39,56, y=65,13, z=380,84], oc['entity.ItemFrame.name'/791, l='MpServer', x=-212,50, y=66,50, z=308,06], oc['entity.ItemFrame.name'/790, l='MpServer', x=-214,50, y=66,50, z=308,06], oc['entity.ItemFrame.name'/789, l='MpServer', x=-216,50, y=66,50, z=308,06], oc['entity.ItemFrame.name'/788, l='MpServer', x=-218,50, y=66,50, z=308,06], oc['entity.ItemFrame.name'/787, l='MpServer', x=-220,50, y=66,50, z=308,06], oc['entity.ItemFrame.name'/786, l='MpServer', x=-222,50, y=66,50, z=308,06], oc['entity.ItemFrame.name'/785, l='MpServer', x=-209,06, y=66,50, z=319,50], rq['Cow'/921, l='MpServer', x=-53,44, y=69,00, z=323,69], oc['entity.ItemFrame.name'/799, l='MpServer', x=-209,06, y=66,50, z=323,50], oc['entity.ItemFrame.name'/798, l='MpServer', x=-209,06, y=66,50, z=321,50], oc['entity.ItemFrame.name'/797, l='MpServer', x=-209,06, y=66,50, z=317,50], oc['entity.ItemFrame.name'/796, l='MpServer', x=-209,06, y=66,50, z=315,50], oc['entity.ItemFrame.name'/795, l='MpServer', x=-209,06, y=66,50, z=313,50], oc['entity.ItemFrame.name'/794, l='MpServer', x=-209,06, y=66,50, z=311,50], te['Creeper'/219299, l='MpServer', x=-14,13, y=65,00, z=301,16], oc['entity.ItemFrame.name'/793, l='MpServer', x=-209,06, y=66,50, z=309,50], oc['entity.ItemFrame.name'/792, l='MpServer', x=-210,50, y=66,50, z=308,06], tv['Zombie'/249700, l='MpServer', x=-15,31, y=65,00, z=305,69], tv['Zombie'/249710, l='MpServer', x=-15,31, y=65,00, z=305,69], te['Creeper'/215629, l='MpServer', x=-25,38, y=66,00, z=295,06], nz['Experience Orb'/261741, l='MpServer', x=-490,53, y=2079,97, z=9781,66], nz['Experience Orb'/261739, l='MpServer', x=-490,58, y=2080,04, z=9782,00], oc['entity.ItemFrame.name'/762, l='MpServer', x=-227,94, y=66,50, z=321,50], oc['entity.ItemFrame.name'/763, l='MpServer', x=-226,50, y=66,50, z=324,94], oc['entity.ItemFrame.name'/760, l='MpServer', x=-224,50, y=66,50, z=324,94], oc['entity.ItemFrame.name'/761, l='MpServer', x=-227,94, y=66,50, z=323,50], oc['entity.ItemFrame.name'/754, l='MpServer', x=-227,94, y=66,50, z=315,50], oc['entity.ItemFrame.name'/755, l='MpServer', x=-227,94, y=66,50, z=313,50], oc['entity.ItemFrame.name'/752, l='MpServer', x=-227,94, y=66,50, z=317,50], oc['entity.ItemFrame.name'/753, l='MpServer', x=-227,94, y=66,50, z=319,50], oc['entity.ItemFrame.name'/758, l='MpServer', x=-226,50, y=66,50, z=308,06], oc['entity.ItemFrame.name'/759, l='MpServer', x=-224,50, y=66,50, z=308,06], oc['entity.ItemFrame.name'/756, l='MpServer', x=-227,94, y=66,50, z=311,50], oc['entity.ItemFrame.name'/757, l='MpServer', x=-227,94, y=66,50, z=309,50], tf['Enderman'/258111, l='MpServer', x=-164,50, y=12,00, z=346,50], tf['Enderman'/258110, l='MpServer', x=-168,50, y=12,00, z=341,50], tv['Zombie'/249785, l='MpServer', x=-15,31, y=65,00, z=305,69], ry['Sheep'/848, l='MpServer', x=-120,84, y=65,00, z=294,92], tv['Zombie'/249791, l='MpServer', x=-15,31, y=65,00, z=305,69]]
	Retry entities: 0 total; []
	Server brand: craftbukkit
	Server type: Non-integrated multiplayer server
Stacktrace:
	at bda.a(SourceFile:284)
	at ats.b(SourceFile:1761)
	at ats.d(SourceFile:633)
	at net.minecraft.client.main.Main.main(SourceFile:101)

-- System Details --
Details:
	Minecraft Version: 1.6.2
	Operating System: Windows XP (x86) version 5.1
	Java Version: 1.7.0_25, Oracle Corporation
	Java VM Version: Java HotSpot(TM) Client VM (mixed mode, sharing), Oracle Corporation
	Memory: 25952304 bytes (24 MB) / 144539648 bytes (137 MB) up to 518979584 bytes (494 MB)
	JVM Flags: 2 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx512M
	AABB Pool Size: 2060 (115360 bytes; 0 MB) allocated, 5 (280 bytes; 0 MB) used
	Suspicious classes: IWrUpdater, Config, WrUpdaterSmooth, ...[bspkrs.client.util.ColorThreshold], [bspkrs.util.ModVersionChecker, BSProp, BSPropRegistry, ...], [com.thevoxelbox.voxelmap.VoxelMap, VoxelRadar, VoxelColorManager, ...], [com.thevoxelbox.voxelmap.gui.GuiMinimapOptions, GuiScreenAddWaypoint], [com.thevoxelbox.voxelmap.gui.overridden.GuiScreenMinimap], [com.thevoxelbox.voxelmap.util.GLBufferedImage, MapData, MapChunkCache, ...]
	IntCache: cache: 0, tcache: 0, allocated: 3, tallocated: 63
	ModLoader: Mods loaded: 6
ModLoader 1.6.2
bspkrsCore v3.03(1.6.2)
StatusEffectHUD v1.14(1.6.2)
StatusEffectHUD v1.14(1.6.2)
ArmorStatusHUD v1.12(1.6.2)
ArmorStatusHUD v1.12(1.6.2)

	Launched Version: Default
	LWJGL: 2.9.0
	OpenGL: GeForce 6150SE nForce 430/integrated/SSE2/3DNOW! GL version 2.1.2, NVIDIA Corporation
	Is Modded: Very likely; Jar signature invalidated
	Type: Client (map_client.txt)
	Resource Pack: faithful32pack.zip
	Current Language: English (US)
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: 885 (49560 bytes; 0 MB) allocated, 35 (1960 bytes; 0 MB) used
