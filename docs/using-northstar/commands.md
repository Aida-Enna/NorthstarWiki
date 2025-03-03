# Commands

### Opening the Console

Commands are run on the console. To open it, press `` ` `` (the key above `TAB`).\
Note that this key generally only exists in this form on English keybords (ANSI US, ISO UK, ...).

If you for example have a German keyboard you'll notice that this key is located left of `BACKSPACE` but won't open the console when you press it.

To open your console you'll either have to switch to the English (US) layout **before** starting the game or rebinding the key to open console.

To rebind it make sure neither Titanfall nor Northstar are running, then go to `My Documents\Respawn\Titanfall2\local\` and open `settings.cfg`.\
Look for the line containing `toggleconsole`, i.e.

```
bind "`" "toggleconsole"
```

and replace the `` ` `` key with your prefered key to open console. So if you want to open console with `F5`, change the line to

```
bind "F5" "toggleconsole"
```

{% hint style="info" %}
In the future this keybind should hopefully be adjustable via `Controls > Settings > Key Binds` from within Titanfall.\
**Note** that if you're using the [Enhanced Menu Mod](https://github.com/taskinoz/Enhanced-Menu-Mod) this might already be the case
{% endhint %}

## List of commands

### Northstar Commands

| Command                 | Result         |
| ----------------------- | -------------- |
| `ns_masterserver_hostname` | Masterserver URL, default: `https://northstar.tf` |
| `ns_auth_allow_insecure 1` | Allows clients to connect without masterserver authorization |
| `connect <ip address>:<port>` | Directly connect to a Northstar gameserver |
| `reload_mods` | Reload mods |
| `ns_disallowed_tacticals` | String list of disallowed tactical abilities, ex: `"mp_ability_grapple,mp_ability_heal"` |
| `ns_disallowed_tactical_replacement` | Optional replacement ability for disallowed tacticals |
| `give mp_weapon_peacekraber` | Gives you peacekraber |

### Server commands

| Variable                                    | Description                                                           | Default |
|---------------------------------------------|-----------------------------------------------------------------------|---------|
| `sv_cheats`                                 | Wether players can use cheat commands (i.e. noclip) .                 | 0       |
| `sv_AllWaysSupportsSaveRestore`             |                                                                       | 0       |
| `sv_allTicksFinal`                          |                                                                       | 0       |
| `sv_allowSendTableTransmitToClients`        |                                                                       | 1       |
| `sv_alltalk`                                | Wether both teams can talk to each other over voice chat.             | 0       |
| `sv_balanceTeams`                           | Wether the server will attempt to keep teams balanced between rounds. | 1       |
| `sv_bounds_show_errors`                     |                                                                       | 0       |
| `sv_clampPlayerFrameTime`                   |                                                                       | 0       |
| `sv_clockcorrection`                        |                                                                       | 1       |
| `sv_clockcorrection_msecs`                  |                                                                       | 75      |
| `sv_compressPlaylists`                      |                                                                       | 1       |
| `sv_connectingClientDelay`                  |                                                                       | 3       |
| `sv_debug_deferred_trace`                   |                                                                       | 0       |
| `sv_debug_deferred_trace_overlay`           |                                                                       | 0       |
| `sv_debug_prop_send`                        |                                                                       | 0       |
| `sv_debugmanualmode`                        |                                                                       | 0       |
| `sv_disconnectOnTooManySnapshotFrames`      |                                                                       | 1       |
| `sv_dumpstringtables`                       |                                                                       | 0       |
| `sv_earlyPersistenceRead`                   |                                                                       | 0       |
| `sv_edgefriction`                           |                                                                       | 2       |
| `sv_everyThirdTick`                         |                                                                       | 0       |
| `sv_extra_client_connect_time`              |                                                                       | 60      |
| `sv_gravity`                                | The amount of gravity the server has.                                 | 750     |
| `sv_hibernate_ms`                           |                                                                       | 5       |
| `sv_hibernate_ms_vgui`                      |                                                                       | 5       |
| `sv_hibernate_postgame_delay`               |                                                                       | 5       |
| `sv_hibernate_when_empty`                   | Wether the server should hibernate when empty.                        | 0       |
| `sv_instancebaselines`                      |                                                                       | 1       |
| `sv_kickPlayersTooFarInFuture`              | Wether to kick players whose internal time is too far  in the future. | 1       |
| `sv_lerpAnims`                              |                                                                       | 1       |
| `sv_lobbyType`                              |                                                                       | 1       |
| `sv_massreport`                             |                                                                       | 0       |
| `sv_maxUserCmdsPerPlayerPerFrame`           |                                                                       | 10      |
| `sv_max_prop_data_dwords_lobby`             |                                                                       | 100000  |
| `sv_max_prop_data_dwords_multiplayer`       |                                                                       | 125000  |
| `sv_max_prop_data_dwords_singleplayer`      |                                                                       | 300000  |
| `sv_max_props_lobby`                        |                                                                       | 50000   |
| `sv_max_props_multiplayer`                  |                                                                       | 75000   |
| `sv_max_props_singleplayer`                 |                                                                       | 200000  |
| `sv_max_snapshots_lobby`                    |                                                                       | 100     |
| `sv_max_snapshots_multiplayer`              |                                                                       | 300     |
| `sv_max_snapshots_singleplayer`             |                                                                       | 10      |
| `sv_maxclientframes`                        |                                                                       | 300     |
| `sv_maxrate`                                |                                                                       | 0       |
| `sv_maxroutable`                            |                                                                       | 1200    |
| `sv_maxupdaterate`                          |                                                                       | 60      |
| `sv_minrate`                                |                                                                       | 128000  |
| `sv_minupdaterate`                          |                                                                       | 20      |
| `sv_noclipaccelerate`                       | The amount of acceleration in noclip.                                 | 10000   |
| `sv_noclipduringpause`                      | Wether to noclip during server pause.                                 | 0       |
| `sv_noclipspeed`                            | The speed for noclip.                                                 | 5       |
| `sv_normalSimulationCommandThreshold`       |                                                                       | 3       |
| `sv_parallel_sendsnapshot`                  |                                                                       | 1       |
| `sv_partyDediOnly`                          |                                                                       | 0       |
| `sv_pausable`                               |                                                                       | 0       |
| `sv_physics_maxvelocity`                    |                                                                       | 4000.0  |
| `sv_playerNameAppendCheater`                |                                                                       | 1       |
| `sv_playerSimTimeBuffer`                    |                                                                       | 0       |
| `sv_precacheinfo`                           |                                                                       |         |
| `sv_printClockCorrections`                  |                                                                       | 0       |
| `sv_printClockTiming`                       |                                                                       | 0       |
| `sv_props_funnel_into_portals`              |                                                                       | 1       |
| `sv_props_funnel_into_portals_deceleration` |                                                                       | 2.0f    |
| `sv_querylimit_per_sec`                     |                                                                       | 10      |
| `sv_quota_stringcmdspersecond`              |                                                                       | 60      |
| `sv_rcon_banpenalty`                        |                                                                       | 0       |
| `sv_rcon_log`                               | Wether to log RCON commands.                                          | 1       |
| `sv_rcon_maxfailures`                       |                                                                       | 10      |
| `sv_rcon_minfailures`                       |                                                                       | 5       |
| `sv_rcon_minfailuretime`                    |                                                                       | 30      |
| `sv_regeneration_wait_time`                 |                                                                       | 20.0    |
| `sv_rejectClientConnects`                   |                                                                       | 0       |
| `sv_rejectConnections`                      |                                                                       | 0       |
| `sv_robust_explosions`                      |                                                                       | 1       |
| `sv_scarySnapDeltaPrints`                   |                                                                       | 50      |
| `sv_screenShake_enabled`                    |                                                                       | 1       |
| `sv_script_think_interval`                  |                                                                       | 0.1     |
| `sv_sendPlaylists`                          |                                                                       | 1       |
| `sv_separate_freq_change_prop_send`         |                                                                       | 1       |
| `sv_shiftPlayerSimTimeBackwards`            |                                                                       | 1       |
| `sv_showClientTickCmds`                     |                                                                       | 0       |
| `sv_showLargeSnapshotSize`                  |                                                                       | 10000   |
| `sv_showLargeSnapshots`                     |                                                                       | 0       |
| `sv_showUserCmds`                           |                                                                       | 0       |
| `sv_show_placement_help_in_preview`         |                                                                       | 0       |
| `sv_showents`                               |                                                                       | 0       |
| `sv_showfiredbullets`                       |                                                                       | 0       |
| `sv_showhitboxes`                           |                                                                       | -1      |
| `sv_showlagcompensation`                    |                                                                       | 0       |
| `sv_shutdown`                               | Shuts down the server.                                                |         |
| `sv_single_core_dedi`                       |                                                                       | 0       |
| `sv_skyname`                                |                                                                       |         |
| `sv_soundscape_printdebuginfo`              |                                                                       |         |
| `sv_specaccelerate`                         |                                                                       | 1000.0  |
| `sv_specnoclip`                             |                                                                       | 1       |
| `sv_specspeed`                              |                                                                       | 5       |
| `sv_stats`                                  |                                                                       | 1       |
| `sv_stressbots`                             |                                                                       | 1       |
| `sv_strugglecheck`                          |                                                                       | 1.016   |
| `sv_teststepsimulation`                     |                                                                       | 0       |
| `sv_thinktimecheck`                         |                                                                       | 0       |
| `sv_threaded_post_process_ai`               |                                                                       | 1       |
| `sv_threaded_post_process_players`          |                                                                       | 1       |
| `sv_turbophysics`                           |                                                                       | 1       |
| `sv_turbophysics_player`                    |                                                                       | 1       |
| `sv_unnecessaryConnectDelay`                |                                                                       | 60      |
| `sv_updaterate_mp`                          |                                                                       | 20      |
| `sv_updaterate_sp`                          |                                                                       | 20      |
| `sv_useReputation`                          |                                                                       | 1       |
| `sv_use_edgefriction`                       |                                                                       | 1       |
| `sv_usercmd_before_entities`                |                                                                       | 1       |
| `sv_usercmd_fairness_dediOnly`              |                                                                       | 0       |
| `sv_usercmd_max_queued`                     |                                                                       | 40      |
| `sv_usercmd_num_per_iteration`              |                                                                       | 1       |
| `sv_usercmd_shuffle_players`                |                                                                       | 1       |
| `sv_visiblemaxplayers`                      |                                                                       | -1      |
| `sv_visualizetraces`                        |                                                                       | 0       |
| `sv_visualizetraces_duration`               |                                                                       | 0.5     |
| `sv_voiceDebug`                             |                                                                       | 0       |
| `sv_voiceEcho`                              |                                                                       | 0       |
| `sv_voiceenable`                            |                                                                       | 1       |
| `sv_warnAboutCmdNumJumps`                   |                                                                       | 20      |
| `sv_weapon_despawn_time`                    |                                                                       | 90      |
| `sv_writeSendTableStreamFile`               |                                                                       |         |

### Useful dev scripts

|Command|Result|
|-|-|
|`script CreateTitanForPlayerAndHotdrop( GetPlayerArray()[0], GetTitanReplacementPoint( GetPlayerArray()[0], false ) )`|Sets your titan as available to call for Titanfall|
|`script ForcePilotToBecomeTitan( GetPlayerArray()[0] )`|Transforms you into a titan|
