# v1.4.2
- Removed changelog field from the `Mod` asset. (#14)

### REPOLib-Sdk v1.2.0
- Added an `Extra Files` field to the `Mod` asset. (REPOLib-Sdk#7)
  - You can put your changelog file here.

## v1.4.1
- Added [`RaiseMasterClient`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Modules/NetworkedEvent.cs#L32) to [`REPOLib.Modules.NetworkingEvents`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Modules/NetworkedEvent.cs) class.
- Added [`RaiseEvent`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Modules/NetworkedEvent.cs#L128) method to [`REPOLib.Modules.NetworkedEvent`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Modules/NetworkedEvent.cs#L101) class.
  - This method works to call in singleplayer.

## v1.4.0
- Added REPOLib as default dependency to the `Mod` asset. (#11)
- Added [`REPOLib.Modules.Utilities`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Modules/Utilities.cs) class that contains a function [`public static void FixAudioMixerGroups(GameObject prefab);`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Modules/Utilities.cs#L28) to fix the audio mixer groups on a prefab and their children. (#10)
- Registering features (Valuables, Items, Enemies, etc...) will now automatically fix their prefabs audio mixer groups.
- Added [`REPOLib.Modules.NetworkedEvent`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Modules/NetworkedEvent.cs#L96) class to easily manage your event codes when using [`PhotonNetwork.RaiseEvent();`](https://doc.photonengine.com/pun/current/gameplay/rpcsandraiseevent) (#12)

## v1.3.1
- Added changelog field to the `Mod` asset. (#9)

## v1.3.0
- Added more validation when registering features to prevent conflicts and errors.
- Added support for registering custom chat /commands. (#5)
  - Added some built-in dev mode commands: `/spawnvaluable <name>`, `/spawnitem <name>` (`/sv` and `/si` for short)
    - You must enable `DeveloperMode` mode in the config settings to use dev mode commands.
    - Note: dev mode commands are host-only!

## v1.2.0
- Added support for registering items.
- Added support for registering enemies. (#2)
- Added support for registering features without code using the [REPOLib-Sdk](https://github.com/ZehsTeam/REPOLib-Sdk). (#3)
- Features now register network prefabs to have their prefabId match the Resources folder structure.
- You can no longer manually pass in a prefabId when registering a valuable.

## v1.1.0
- You can now register valuables to specific levels. (#1)
  - Valuables Presets: `Valuables - Generic`, `Valuables - Wizard`, `Valuables - Manor`, `Valuables - Arctic`

## v1.0.2
- Small improvement to [`NetworkPrefabs.cs`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Modules/NetworkPrefabs.cs), [`Valuables.cs`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Modules/Valuables.cs), [`CustomPrefabPool.cs`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Objects/CustomPrefabPool.cs), [`LevelValuablesExtension.cs`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Extensions/LevelValuablesExtension.cs), and other.
- Added `public static IReadOnlyList<GameObject> RegisteredValuables { get; }` to [`Valuables.cs`](https://github.com/ZehsTeam/REPOLib/blob/main/REPOLib/Modules/Valuables.cs#L11)

## v1.0.1
- Updated mod icon.

## v1.0.0
- Initial release.