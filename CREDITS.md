# Third-party credits

Kelgekeman includes the following credited assets. The descriptions below identify their sources and adaptations; use does not imply endorsement by their authors.

## GrassAndWeeds

Grass and weeds
By Beccasaurus (beccastabler)
https://sketchfab.com/beccastabler
https://sketchfab.com/3d-models/grass-and-weeds-344af319c15d42da9e33d16bb534d95f
Licensed under Creative Commons Attribution 4.0 International (CC BY 4.0).
https://creativecommons.org/licenses/by/4.0/

Source package supplied by the user: grass-and-weeds.zip.
The original base-color, normal and ambient-occlusion images are unchanged.
Adaptations: configured for Unity URP with repeating, filtered textures, a shared
world-aligned ground material, reduced normal/AO intensity and matte lighting.
The supplied FBX display plinth is not used as terrain. Original texture maps,
including roughness, are retained in ArtSource/GrassAndWeeds.


## TreeAnimate

Tree Animate
By RandyGF (https://sketchfab.com/RandyGF)
https://sketchfab.com/3d-models/tree-animate-f0f9eb5e6c104bbb8e1f41c97019e6f2
Creative Commons Attribution 4.0 International (CC BY 4.0).
http://creativecommons.org/licenses/by/4.0/
Attribution and license are embedded in the user-supplied tree_animate.glb metadata.

Game adaptations: separated the three spatially arranged trees into standalone
FBX variants, preserving source UVs and all five leaf/branch morph targets.
Original bark, leaf and branch color/normal maps are unchanged. Leaf and branch
materials are double-sided alpha cutouts with mip coverage preservation.
Source wind samples are replayed on visible nearby trees, with varied start times.
The models are centered, grounded and normalized for existing decorative and
clearable trees. Orchard/crop trees and progression rules are unchanged.
Original.glb and the reproducible conversion scripts are in ArtSource/TreeAnimate.

Foliage uses URP Simple Lit with specular highlights disabled. Leaf normal-map sampling is disabled to preserve the source foliage color on the animated cutout cards. The leaf normal image remains unchanged in the source and imported assets. Camera fading scales the cutout threshold with opacity so leaves do not pop out abruptly.


## JeepWillys

Jeep Willys Pickup

This work is based on "Jeep Willys Pickup" (https://sketchfab.com/3d-models/jeep-willys-pickup-9abffd2c23af48f1b77ea786a5917efd) by jvouillon (https://sketchfab.com/jvouillon), licensed under CC-BY-4.0 (https://creativecommons.org/licenses/by/4.0/).

Game adaptations: converted to FBX, centered and scaled to the existing truck footprint, trimmed the bottom ground skirt, reduced mesh density, combined the texture pages into one atlas, and configured a material for Unity URP. This notice is included in StreamingAssets/ThirdPartyNotices for future builds.


## RockMountainCave

Rock Mountain with cave (realistic version)
By Jungle Jim (jungle_jim)
https://sketchfab.com/jungle_jim
https://sketchfab.com/3d-models/rock-mountain-with-cave-realistic-version-184293c4ef6f49daa06ea2654a40b6ed
Model listing license: Creative Commons Attribution 4.0 International (CC BY 4.0).
https://creativecommons.org/licenses/by/4.0/
The author describes the texture source as Quixel.

Source archive supplied by the user: rock-mountain-with-cave-realistic-version.zip.
The ZIP contains three different PNG entries with the same filename. All were
preserved by entry order in ArtSource/RockMountainCave to avoid overwriting them:
texture-1: roughness; texture-2: base color; texture-3: metallic; texture-4: normal.
The included FBX names the normal, roughness and metallic texture channels.
The original source.fbx is preserved outside Unity's runtime assets.

Game adaptation: unchanged source base color, normal and roughness maps imported
at 4096 maximum resolution. Shared non-metallic URP world-space triplanar material
applied to the existing cave arch, jambs, mountain core and eroded outcrops.
A rock-only square within the atlas is sampled using mirrored repeats to avoid
empty UV-island padding. No generated/repainted texture was substituted.
Atlas square in source pixel coordinates (top-left origin): x=760, y=1640,
width=1200, height=1200. This same atlas region and normal orientation are used
on every projected face; one repeat spans five world units.
The metallic map is preserved as source but not used for the mountain's stone.


Cave entrance model adaptation (2026-11-03): the original source FBX is now
imported as Assets/Game/Art/CaveEntrance/RockMountainCave.fbx and authored into
Resources/Scenery/CaveEntrance.prefab. The original mesh and UV atlas replace
the former constructed stone arch, rails, lanterns and tunnel-shadow polygon.
The source opening faces the meadow, is aligned to the existing cave travel
point, and has mesh collision. Its base shelf is buried at meadow level.
The entrance uses the complete source albedo and normal maps with a matte URP
material. Surrounding generated mountain rocks retain the matching triplanar
material, with space reserved for the imported entrance.


Entrance model reverted at the user's request (2026-11-03). The previous
stone arch, rails, lanterns and surrounding rock arrangement are restored.
The pack's rock textures remain on the arch and mountain. The imported entrance
prefab is retained outside Resources as an unused editable asset.


## EmeraldSword

Stylized Emerald Sword
Matheus Elias (https://sketchfab.com/Tuteupai)
https://sketchfab.com/3d-models/stylized-emerald-sword-c54f6718314a4416887e231271bb4da0
License: CC-BY-4.0 (http://creativecommons.org/licenses/by/4.0/)
Changes: converted supplied GLB to a shared Unity mesh and URP material; reoriented, resized and positioned for the existing two-handed sword grip.


## Text and interface libraries

- [RTLTMPro](https://github.com/pnarimani/RTLTMPro), by Peyman Narimani, MIT license. [License notice](LICENSES/RTLTMPro-MIT.txt).
- [UIEffect](https://github.com/mob-sakai/UIEffect), by mob-sakai. See the project's license and copyright notice in the linked source repository.
- Noto Naskh Arabic and the renamed Kelgekeman Naskh derivative use the SIL Open Font License. [Font license](LICENSES/Noto-OFL.txt).
- Unity and TextMeshPro are used under their respective Unity license terms.

The app icon is original AI-generated artwork prepared for Kelgekeman. It is illustrative branding, not a gameplay screenshot.
