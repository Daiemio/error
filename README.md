Exception in Verse.PawnRenderer.RenderCache: System.NullReferenceException: Object reference not set to an instance of an object

  at Verse.GenDraw.DrawMeshNowOrLater (UnityEngine.Mesh mesh, UnityEngine.Vector3 loc, UnityEngine.Quaternion quat, UnityEngine.Material mat, System.Boolean drawNow) [0x00043] in <b64badbf3c3d41018b3ca5d3e8c77771>:0 
  
     - prefix Torann.ARimworldOfMagic: Boolean TorannMagic.TorannMagicMod+DrawMesh_Cloaks_Patch:Prefix(Mesh mesh, Vector3 loc, Quaternion quat, Material mat, Boolean drawNow)
  
  at Verse.PawnRenderer.DrawPawnBody (UnityEngine.Vector3 rootLoc, System.Single angle, Verse.Rot4 facing, Verse.RotDrawMode bodyDrawType, Verse.PawnRenderFlags flags, UnityEngine.Mesh& bodyMesh) [0x001a3] in <b64badbf3c3d41018b3ca5d3e8c77771>:0
  
     - transpiler rimworld.erdelf.alien_race.main: IEnumerable`1 AlienRace.HarmonyPatches:DrawPawnBodyTranspiler(IEnumerable`1 instructions)
  
     - prefix Torann.ARimworldOfMagic: Boolean TorannMagic.TorannMagicMod+PawnRenderer_Undead_Prefix:Prefix(PawnRenderer __instance, Vector3 rootLoc, Single angle, Rot4 facing, RotDrawMode& bodyDrawType, PawnRenderFlags flags, Pawn ___pawn, Mesh& bodyMesh)
  
  at Verse.PawnRenderer.RenderPawnInternal (UnityEngine.Vector3 rootLoc, System.Single angle, System.Boolean renderBody, Verse.Rot4 bodyFacing, Verse.RotDrawMode bodyDrawType, Verse.PawnRenderFlags flags) [0x001eb] in <b64badbf3c3d41018b3ca5d3e8c77771>:0 
  
     - transpiler rimworld.erdelf.alien_race.main: IEnumerable`1 AlienRace.HarmonyPatches:RenderPawnInternalTranspiler(IEnumerable`1 instructions)
  
     - transpiler rimworld.Nals.FacialAnimation: IEnumerable`1 FacialAnimation.HarmonyPatches:TranspilerInsertAnimationHeadCode(IEnumerable`1 instructions)
  
     - transpiler net.velc.rimworld.mod.hds: IEnumerable`1 HatDisplaySelection.Patch:Transpiler_PawnRenderer_RenderPawnInternal(IEnumerable`1 instructions)
  
     - prefix rimworld.torann.tmagic: Boolean TorannMagic.TorannMagicMod:PawnRenderer_UndeadInternal_Prefix(PawnRenderer __instance, Vector3& rootLoc, Single angle, Boolean renderBody, Rot4 bodyFacing, RotDrawMode& bodyDrawType, PawnRenderFlags flags, Pawn ___pawn, PawnGraphicSet ___graphics)
  
     - prefix Altered.Carbon: Void AlteredCarbon.Rotation_Patch+PawnRenderer_RenderPawnInternal_Patch:Prefix(Pawn ___pawn, Vector3 rootLoc, Single angle, Boolean renderBody, Rot4 bodyFacing, RotDrawMode bodyDrawType, PawnRenderFlags flags)
  
     - prefix rimworld.jecrell.vampire: Boolean Vampire.HarmonyPatches:RenderVampire(PawnRenderer __instance, Vector3 rootLoc, Single angle, Boolean renderBody, Rot4 bodyFacing, RotDrawMode bodyDrawType, PawnRenderFlags flags)
  
     - prefix rimworld.Nals.FacialAnimation: Boolean FacialAnimation.HarmonyPatches:PrefixRenderPawnInternal(Rot4 bodyFacing, RotDrawMode bodyDrawType, PawnRenderFlags& flags, Pawn& ___pawn)
  
     - prefix net.velc.rimworld.mod.hds: Boolean HatDisplaySelection.Patch:Patch_PawnRenderer_RenderPawnInternal_Initialize(PawnRenderer __instance, Pawn ___pawn, Vector3 rootLoc, Single angle, Boolean renderBody, Rot4 bodyFacing, RotDrawMode bodyDrawType, PawnRenderFlags flags)
  
     - postfix rimworld.Nals.FacialAnimation: Void FacialAnimation.HarmonyPatches:PostfixRenderPawnInternal()
  
     - postfix net.velc.rimworld.mod.hds: Void HatDisplaySelection.Patch:Patch_PawnRenderer_RenderPawnInternal(PawnRenderer __instance, Pawn ___pawn, Vector3 rootLoc, Single angle, Boolean renderBody, Rot4 bodyFacing, RotDrawMode bodyDrawType, PawnRenderFlags flags)
  
  at Verse.PawnRenderer.RenderCache (Verse.Rot4 rotation, System.Single angle, UnityEngine.Vector3 positionOffset, System.Boolean renderHead, System.Boolean renderBody, System.Boolean portrait, System.Boolean renderHeadgear, System.Boolean renderClothes, System.Collections.Generic.Dictionary`2[TKey,TValue] overrideApparelColor, System.Nullable`1[T] overrideHairColor, System.Boolean stylingStation) [0x00186] in <b64badbf3c3d41018b3ca5d3e8c77771>:0 
  
     - transpiler net.pardeike.rimworld.lib.harmony: IEnumerable`1 VisualExceptions.ExceptionsAndActivatorHandler:Transpiler(IEnumerable`1 instructions, MethodBase original)
