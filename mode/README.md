# GCRP Data Pack v4 — Faction & OCG Skins

61 custom skins (31 male + 30 female) integrated into the client data pack.
They replace the stock skin IDs below (unused-by-shop skins; verify none of
your active player skins collide — re-mapping is a 5-minute rebuild).

| Organization | Gender | Ranks | SKIN ID (SetPlayerSkin) |
|---|---|---|---|
| Yuzhny Police Department | Female | 1-4 | **65** |
| Yuzhny Police Department | Female | 5-8 | **10** |
| Yuzhny Police Department | Female | 9-10 | **12** |
| Yuzhny Police Department | Male | 1-4 | **1** |
| Yuzhny Police Department | Male | 5-8 | **2** |
| Yuzhny Police Department | Male | 9-10 | **3** |
| Yuzhny Hospital | Female | 1-4 | **31** |
| Yuzhny Hospital | Female | 5-8 | **39** |
| Yuzhny Hospital | Female | 9-10 | **40** |
| Yuzhny Hospital | Male | 1-4 | **4** |
| Yuzhny Hospital | Male | 5-8 | **5** |
| Yuzhny Hospital | Male | 9-10 | **6** |
| Government | Female | 1-4 | **41** |
| Government | Female | 5-8 | **53** |
| Government | Female | 9-10 | **55** |
| Government | Male | 1-2 | **8** |
| Government | Male | 3-4 | **42** |
| Government | Male | 5-8 | **86** |
| Government | Male | 9-10 | **149** |
| Military | Female | 1-4 | **56** |
| Military | Female | 5-8 | **87** |
| Military | Female | 9-10 | **141** |
| Military | Male | 1-4 | **208** |
| Military | Male | 5-8 | **273** |
| Military | Male | 9-10 | **14** |
| News Network | Female | 1-4 | **172** |
| News Network | Female | 5-8 | **190** |
| News Network | Female | 9-10 | **191** |
| News Network | Male | 1-4 | **15** |
| News Network | Male | 5-8 | **18** |
| News Network | Male | 9-10 | **22** |
| Secret Intelligence Authority | Female | 1-4 | **195** |
| Secret Intelligence Authority | Female | 5-8 | **197** |
| Secret Intelligence Authority | Female | 9-10 | **211** |
| Secret Intelligence Authority | Male | 1-4 | **24** |
| Secret Intelligence Authority | Male | 5-8 | **25** |
| Secret Intelligence Authority | Male | 9-10 | **32** |
| OCG Vega | Female | 1-4 | **216** |
| OCG Vega | Female | 5-8 | **219** |
| OCG Vega | Female | 9-10 | **224** |
| OCG Vega | Male | 1-4 | **33** |
| OCG Vega | Male | 5-8 | **35** |
| OCG Vega | Male | 9-10 | **37** |
| OCG Argon | Female | 1-4 | **226** |
| OCG Argon | Female | 5-8 | **84** |
| OCG Argon | Female | 9-10 | **82** |
| OCG Argon | Male | 1-4 | **44** |
| OCG Argon | Male | 5-8 | **45** |
| OCG Argon | Male | 9-10 | **49** |
| OCG Drago | Female | 1-4 | **23** |
| OCG Drago | Female | 5-8 | **95** |
| OCG Drago | Female | 9-10 | **96** |
| OCG Drago | Male | 1-4 | **51** |
| OCG Drago | Male | 5-8 | **52** |
| OCG Drago | Male | 9-10 | **58** |
| OCG Grom | Female | 1-4 | **97** |
| OCG Grom | Female | 5-8 | **101** |
| OCG Grom | Female | 9-10 | **132** |
| OCG Grom | Male | 1-4 | **59** |
| OCG Grom | Male | 5-8 | **61** |
| OCG Grom | Male | 9-10 | **62** |

## Replaced stock skin IDs (full list)

1, 2, 3, 4, 5, 6, 8, 10, 12, 14, 15, 18, 22, 23, 24, 25, 31, 32, 33, 35, 37, 39, 40, 41, 42, 44, 45, 49, 51, 52, 53, 55, 56, 58, 59, 61, 62, 65, 82, 84, 86, 87, 95, 96, 97, 101, 132, 141, 149, 172, 190, 191, 195, 197, 208, 211, 216, 219, 224, 226, 273

## PAWN usage
```pawn
#include "faction.in"
#include "ocg.in"

// on spawn / promote:
SetPlayerSkin(playerid, GCRP_FactionSkin(GCRP_FACTION_YPD, GCRP_SKIN_MALE, GetPVarInt(playerid, "rank")));
SetPlayerSkin(playerid, GCRP_OcgSkin(GCRP_OCG_VEGA, GCRP_OCG_FEMALE, 9));
// or use the #defines directly: GCRP_SKIN_YPD_MALE_R9_10 etc.
```
