# PublicUnknown's Battlegrounds
A BATTLE ROYALE MULTIPLAYER GAME UE4 PROJECT

Template Overview:
https://vk.com/video-205432676_456239124
![Screenshot](07.PNG)
![Screenshot](05.PNG)
![Screenshot](01.PNG)
![Screenshot](02.PNG)
![Screenshot](03.PNG)
![Screenshot](06.PNG)

## PUBLIC UNKNOWN'S LITE CODE STRUCTURE

![Screenshot](Code3.PNG)

' Base Unreal Engine classes
class UObject
class AActor {
}
class UActorComponent {
}
class UUserWidget {
}

' tsl Lite main module, 
' '  Survive sub module package

package Survive {
    package Plugins {
        package GVoiceSDK {
            class GVoiceSDK
        }
        package OceanPlugin {
            class BuoyancyForceComponent
            class OceanManager
            class BuoyantMeshComponent
            class WaterHeightmapComponent
        }
        package tslLauncher {
            class tslLauncher
        }
        package RuntimeMeshComponent {
            class RuntimeMeshComponent
            class RuntimeMeshCore
        }
        package SkillEditor {
            class UTSkill
            class UTSkillManagerComponent
            class UTSkillPhase
        }
        package TApm {
            class TApmHelper
        }
        package UAETrigger {
            class UAELevelDirector
            class UAETriggerObject
            class LevelEventCenter
            class TriggersFlowTree
        }
        package WWise {
            class AkAudioDevice
            class AkComponent
            class AkComponentCallbackManager
            class AkGameplayStatics
            class AkFilePackagerLowLevelIO
        }
    }

    package Source {
        package Basic {
            package Buff {
                class STBaseBuffSystemComponent
            }
            class AttrModifyComponent
            class BattleItem
            class BPClassManager
            class ItemContainer
            class PackTool
            class UAEGameEngine
            class UAELoadedClassManager
            class UAENetConnection
            class UAENetDriver
            class UAETableManager
            class UAEVersion
        }

        package Client {
            package BpToolLib {
                class BusinessHelper
            }
            package HotUpdate {
                class HotUpdater
            }
            package Private {
                class GameBackendHUD
                class GameBusinessManager
                class GameFrontendHUD
                class InGameUIManager
                class LuaClassObj
                class TssManager
            }
            package ScriptHelp {
                class ScriptHelperClient
            }
            package Tools {
                class GVoiceInterface
                class LoadTexture
            }
            package Widgets {
                class SUTRichTextBlock
                class UAERichTextBlock
            }
        }

        package Gameplay {
            class BackpackComponent
            class BaseGeneratorComponent
            class ChaVehAnimListComponent
            class GlobalConfigActor
            class ItemGeneratorComponent
            class ItemSpotSceneComponent
            class UAECharacter
            class UAECharacterAnimListComponent
            class UAEGameMode
            class UAEHouseActor
            class UAEOBState
            class UAEPlayerController
            class UAEPlayerState
            class UAEProjectile
            class VehicleSpotSceneComponent
        }

        package ShadowTrackerExtra {
            class STExtraGameInstance
            class STExtraGameMode
            class STExtraGameplayStatics

            package Animation {
                class STExtraAnimInstance
            }
            package BackPack {
                class BackpackAvatarItem
                class BackpackAvatarItemCustom
                class BackpackUtils
                class BackpackWeaponAttachHandle
            }
            package Buff {
                class STExtraBuffAction_AdjustStunPostMat
                class STExtraBuffAction_DrowningDamage
            }
            package Caching {
                class CachingManager
            }
            package ChallengeLevel {
                class DrivingChallengeLevelRules
                class OnTimeSpawnChallengeLevelRules
            }
            package Character {
                class CharacterWeaponManagerComponent
                class SceneCaptureCharacter
                class STCharacterFollowComp
                class STCharacterMovementComponent
                class STCharacterNearDeathComp
                class STCharacterRescueOtherComp
                class STExtraBaseCharacter
            }
            package Chat {
                class ChatComponent
            }
            package CustomActor {
                class AirDropBoxActor
                class AirDropPlane
                class CircleAreaVolume
                class tslDoor
            }
            package CustomComponent {
                class AirAttackComponent
                class AirAttackCS
                class AirDropComponent
                class AvatarComponent
                class CharacterAvatarComponent
                class CircleMgrComponent
                class CommonBtnComponent
                class CustomParticleSystemComponent
                class GameEventListener
                class LandScapeLODByHeight
                class NewbieGuideComponent
                class ParachuteFollowComponent
                class PlaneComponent
                class SecuryInfoComponent
                class ServerSwitchComponent
                class STExtraUnderWaterEffectComp
                class STScreenAppearanceComponent
                class TimerRegistComponent
                class VehicleSpringArmComponent
                class WeaponAvatarComponent
            }
            package Effect {
                class Effect
                class EffectComponent
                class EffectConsumeItem
                class EffectDamage
                class EffectGraph
                class EffectRefreshWeapon
                class EffectReloadWait
                class EffectTakeItem
                class EffectWait
                class EffectWeaponCheckReload
            }
            package Game {
                class STExtraGameStateBase
            }
            package GameMode {
                class BattleRoyaleGameMode
                class BattleRoyaleGameModeGroup
                class BattleRoyaleGameModeTeam
                class DeathMatchGameMode
                class DeathMatchGameState
                class FreeForAllGameMode
                class GameModeDataAsset
                class GameModeStateActive
                class GameModeStateEmpty
                class GameModeStateFighting
                class GameModeStateFinished
                class GameModeStateFinishedGroup
                class GameModeStateFinishedTeam
                class GameModeStateFinishedWar
                class GameModeStateFlying
                class GameModeStateFlyingGroup
                class GameModeStateFlyingTeam
                class GameModeStateFlyingWar
                class GameModeStateReady
                class GameModeState_Challenge
                class GameModeState_Training
                class WarGameMode

                package FreeForAllMatch {
                    class GameModeStateActive_FreeForAll
                    class GameModeStateFighting_FreeForAll
                    class GameModeStateFinished_FreeForAll
                    class GameModeStateReady_FreeForAll
                }
                package TeamMatch {
                    class GameModeStateActive_TeamMatch
                    class GameModeStateFighting_TeamMatch
                    class GameModeStateFinished_TeamMatch
                    class GameModeStateReady_TeamMatch
                    class GameModeStateStartScene_TeamMatch
                }
            }
            package GunPlay {
                class AimingComp
            }
            package Landscape {
                class MyLandscape
            }
            package Online {
                class STExtraGameSession
                class STExtraOnlineSession
            }
            package Option {
                class TslGameUserSettings
            }
            package Pickup {
                class PickupManagerComponent
            }
            package Player {
                class AutoRunTest
                class AutoRunTestInfoOut
                class PlayerControllerStateActive
                class PlayerControllerStateFighting
                class PlayerControllerStateFinished
                class PlayerControllerStateFlying
                class PlayerControllerStateJumping
                class PlayerControllerStateLanding
                class PlayerControllerStateMachine
                class STExtraPlayerCharacter
                class STExtraPlayerController
                class STExtraPlayerController_Spectator
                class STExtraPlayerScreenCheck
                class STExtraPlayerState
                class VehicleUserComponent

                package ItemAvatarComponent {
                    class ItemAvatarComponentBase
                    class VehicleAvatarComponent
                }
            }
            package Private {
                class GMCheatManager
                class HackReporterComponent
                class InteractorComponent
                class LPCLevelScriptActor
                class TargetKeyOperation
                class TslStatics
                class TslWebSocket

                package AI {
                    package Assist {
                        class AIActingComponent
                        class AIWorldVolume
                        class UAEAIOcclusion
                        class UAERecastNavMesh
                    }
                    package Component {
                        class NewPathFollowingComponent
                    }
                    package Controller {
                        class BaseAIController
                        class FakePlayerAIController
                    }
                    package Service {
                        class BTService_AdvancedShooting
                    }
                    package Task {
                        class BTTaskNode_EquipOrUnWeapon
                        class BTTaskNode_FindItemSpot
                        class BTTaskNode_NewParachuteJump
                        class BTTaskNode_ParachuteJumpV3
                        class BTTaskNode_PickItemsAtSpot
                        class BTTask_Escape
                        class BTTask_MoveAround
                        class BTTask_MoveToOcclusion
                        class BTTask_PickUpItemAtTombBox
                        class BTTask_TeleportToSpecLoc
                    }
                }
                package AntiCheat {
                    package SteamNetworkStatusControl {
                        class SteamNetworkStatusControl
                    }
                    package Xenuine {
                        class XenuineHelper
                    }
                }
                package InterfaceForLobbyLink {
                    class GameInstanceForLobbyLink
                    class GameModeForLobbyLink
                }
                package Online {
                    class TslLPCGameMode
                    class TslPCPlayerState
                }
                package Tests {
                    class AutoRunPlayerTestActor
                }
                package Trigger {
                    package Action {
                        class TriggerAction_PrintMsg
                    }
                    package Item {
                        class TriggerItem_TriggerClock
                    }
                }
                package UI {
                    class CoherentCommonBinder
                    class LobbyHUD
                    class TslBaseHUD
                    interface TslNaviWidgetInterface
                    package HUD {
                        class TslBoostGaugeWidget
                    }
                }
            }

            package Props {
                class ItemGeneratorBase
                class PickUpListWrapperActor
                class PickUpWrapperActor
                class PlayerTombBox
                class STExtraProp
            }
            package Replay {
                class DeathPlayback
                class WonderfulRecordingCut
            }
            package Security {
                class SecurityLogWeaponCollector
            }
            package Skill {
                class UAEBaseSkill
                class UAESkill
                class UAESkillAction_AttachActor
                class UAESkillAction_BreakGlass
                class UAESkillAction_PlayMontage
                class UAESkillAction_ReplaceCharAnim
                class UAESkillAction_SetRecoveryPrompt
                class UAESkillAction_ShowSkillPrompt
                class UAESkillAction_TakeDamage
                class UAESkillPicker_Fan
                class UAESkillPicker_FanForClient
                class UTSkillAppearance_SoundCue
            }
            package Templates {
                class TemplateMgr
                class TemplateUtil
            }
            package UI {
                class VoiceCheckObject
                package KeyHint {
                    package KeyboardAndMouse {
                        class TslKeyboardAndMouseHintWidget
                    }
                }
                package Widget {
                    class CustomScrollBox
                    class ParachutingWidget
                    class SCustomScrollBox
                    class SRadarChartUserWidget
                }
            }
            package Utility {
                class ActorCacheMgr
                class BitMsg
                class STExtraBlueprintFunctionLibrary
                class STExtraMapFunctionLibrary
                class STExtraUIUtils
            }
            package Vehicle {
                class STExtraVehicleBase
                class STExtraVehicleUtils
                class VehicleDamageComponent
                class VehicleSeatComponent
                class VehicleSyncComponent

                package Wheeled {
                    class STExtraVehicleMovementComponent4W
                    class STExtraWheeledVehicle
                }
            }
            package Weapons {
                class FireWeaponState
                class IdleWeaponState
                class STEFlareGunProjectComponent
                class STEShootWeaponProjectComponent
                class STExtraShootWeapon
                class STExtraShootWeaponComponent
                class STExtraWeapon
                class WeaponAntiCheatComp
                class WeaponManagerComponent
                class WeaponPostFireState
                class WeaponPreFireState
                class WeaponSpecificHandler
                class WeaponStateManager
            }
        }

        package ThirdParty {
            package BGPrimary {
                class BGPrimary
                class BGPrimaryRunnable
            }
            package Discord {
                class BGDiscord
            }
        }

        package TslCommon {
            class TslGameLog
            class TslWebSocket
            class TslWebSocketRunnable
        }

        package UnrealArchExt {
            class BackendHUD
            class FrontendHUD
            class LogicManagerBase
            class UAEUserWidget
        }
    }
}

' Inheritance (Unreal typical)
UObject <|-- AActor
UObject <|-- UActorComponent
UObject <|-- UUserWidget

AActor <|-- Survive::Source::Gameplay::UAECharacter
AActor <|-- Survive::Source::Gameplay::UAEHouseActor
AActor <|-- Survive::Source::Gameplay::UAEProjectile
AActor <|-- Survive::Source::Gameplay::CustomActor::AirDropBoxActor
AActor <|-- Survive::Source::Gameplay::CustomActor::AirDropPlane
AActor <|-- Survive::Source::Gameplay::CustomActor::tslDoor
AActor <|-- Survive::Source::Gameplay::Props::PickUpListWrapperActor
AActor <|-- Survive::Source::Gameplay::Props::PickUpWrapperActor
AActor <|-- Survive::Source::Gameplay::Props::PlayerTombBox

UActorComponent <|-- Survive::Source::Gameplay::BackpackComponent
UActorComponent <|-- Survive::Source::Gameplay::BaseGeneratorComponent
UActorComponent <|-- Survive::Source::Gameplay::ItemGeneratorComponent
UActorComponent <|-- Survive::Source::Gameplay::ItemSpotSceneComponent
UActorComponent <|-- Survive::Source::Gameplay::VehicleSpotSceneComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::AirAttackComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::AirDropComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::AvatarComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::CharacterAvatarComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::CircleMgrComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::CommonBtnComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::CustomParticleSystemComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::GameEventListener
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::LandScapeLODByHeight
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::NewbieGuideComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::ParachuteFollowComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::PlaneComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::SecuryInfoComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::ServerSwitchComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::STExtraUnderWaterEffectComp
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::STScreenAppearanceComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::TimerRegistComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::VehicleSpringArmComponent
UActorComponent <|-- Survive::Source::Gameplay::CustomComponent::WeaponAvatarComponent

UUserWidget <|-- Survive::Source::Client::Widgets::SUTRichTextBlock
UUserWidget <|-- Survive::Source::Client::Widgets::UAERichTextBlock
UUserWidget <|-- Survive::Source::UnrealArchExt::UAEUserWidget
UUserWidget <|-- Survive::Source::Client::UI::KeyHint::KeyboardAndMouse::TslKeyboardAndMouseHintWidget
UUserWidget <|-- Survive::Source::Client::UI::Widget::CustomScrollBox
UUserWidget <|-- Survive::Source::Client::UI::Widget::ParachutingWidget
UUserWidget <|-- Survive::Source::Client::UI::Widget::SCustomScrollBox
UUserWidget <|-- Survive::Source::Client::UI::Widget::SRadarChartUserWidget

' Associations ()
Survive::Source::Gameplay::UAECharacter --> Survive::Source::Gameplay::BackpackComponent : has
Survive::Source::Gameplay::UAECharacter --> Survive::Source::Gameplay::UAECharacterAnimListComponent : uses
Survive::Source::Gameplay::UAEPlayerController --> Survive::Source::Gameplay::UAEPlayerState : manages
Survive::Source::Gameplay::UAEGameMode --> Survive::Source::Gameplay::UAEPlayerController : controls
Survive::Source::Gameplay::UAEGameMode --> Survive::Source::Gameplay::UAEPlayerState : manages
Survive::Source::Gameplay::UAEGameMode --> Survive::Source::Gameplay::UAECharacter : spawns
Survive::Source::Gameplay::WeaponManagerComponent --> Survive::Source::Gameplay::STExtraShootWeapon : manages
Survive::Source::Gameplay::STExtraShootWeapon --> Survive::Source::Gameplay::FireWeaponState : uses
Survive::Source::Gameplay::STExtraShootWeapon --> Survive::Source::Gameplay::IdleWeaponState : uses

' Core
class GameMode {
    +StartMatch()
    +EndMatch()
    +HandlePlayerDeath()
}

class PlayerController {
    +ProcessInput()
    +SwitchState(State)
    +Health : float
    +State : PlayerControllerState
}

class PlayerCharacter {
    +Move()
    +Jump()
    +FireWeapon()
    +Health : float
    +Armor : float
    -Inventory : InventoryComponent
}

class InventoryComponent {
    +AddItem(Item)
    +RemoveItem(Item)
    -Items : Item[]
}

class Item {
    +Use()
    +Type : ItemType
}

class Weapon {
    +Fire()
    +Reload()
    +Ammo : int
    +Damage : float
}

class Vehicle {
    +Drive()
    +Enter()
    +Exit()
    +Health : float
    +Fuel : float
}

class AIController {
    +PlanRoute()
    +DecideAction()
    +BehaviorTree : BehaviorTree
}

class GameState {
    +GetCurrentState()
    +SetCurrentState(State)
    -CurrentState : GameStateType
}

class UIManager {
    +ShowHUD()
    +UpdateInventoryDisplay()
}

class SkillSystem {
    +ActivateSkill(Skill)
    +CooldownComplete(Skill)
}

class MatchmakingSystem {
    +FindMatch()
    +JoinTeam()
}

' Relationships
PlayerController --> PlayerCharacter : controls
PlayerCharacter --> InventoryComponent : uses
PlayerCharacter --> Weapon : equips
PlayerCharacter --> Vehicle : interacts
AIController --> PlayerCharacter : targets
GameMode --> GameState : maintains
GameMode --> MatchmakingSystem : coordinates
UIManager --> PlayerController : updates
SkillSystem --> PlayerCharacter : interacts

' Components
package "Client Components" {
    [PlayerController]
    [UIManager]
    [InventoryComponent]
}

package "Gameplay Systems" {
    [GameMode]
    [SkillSystem]
    [MatchmakingSystem]
    [PlayerCharacter]
}

package "AI System" {
    [AIController]
}

package "Networking" {
    [NetworkManager]
}

package "Third-party Plugins" {
    [GVoiceSDK]
    [OceanPlugin]
}

' Interfaces
[NetworkManager] --> [GVoiceSDK] : integrates
[GameMode] --> [NetworkManager] : manages
[PlayerController] --> [UIManager] : updates UI
[PlayerCharacter] --> [InventoryComponent] : has
[AIController] --> [PlayerCharacter] : interacts

client Player
participant "PlayerController" as PC
participant "PlayerCharacter" as Character
participant "Weapon" as Weapon

Player -> PC : Press Fire Button
PC -> Character : Trigger FireWeapon()
Character -> Weapon : Fire()
Weapon -> Character : Decrease Ammo
Character -> PC : Update HUD

