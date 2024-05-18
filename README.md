# Hooked ThirdPersonGameMode

Contains hooks that run when the game starts (not including menus).

### Contribution rules

To keep this project backwards compatible with supported mods, this project is __append only__. In other words, contributors are not allowed to delete or modify any hooks that already exist.

### How to add a hook

1. In your mod project (not this project), create a blueprint. Make it an actor component.
1. In _this_ project, add a dummy of that blueprint actor component (i.e. same path, same asset name).
1. In `/Game/Blueprints/GameData/BP_ThirdPersonGameMode`, add the actor component you just dummied.

Congratulations, you now have a hook into the game!

### How to build

Prerequisites:

- Unreal Engine 5.1
- Python 3

1. Run `cook.bat`
1. Run `deploy.bat`
1. Run the game
