# Conquest SMP Integrations

Companion configuration for Paper 1.21.11 and Conquest SMP Mass.

The GrimAC profile records alerts and local history without automatic ban or kick commands. Movement checks may still correct invalid movement. No profile can guarantee zero false positives. Review alerts before staff action.

Install King's Crown separately for crown integration. Install official Geyser-Spigot and Floodgate builds and configure a host-provided UDP port for Bedrock. Keep Floodgate private keys private. Conquest contains the integration hooks and update support. Authentication and player identity settings are deployment-specific and are deliberately not included here.

Conquest SMP 3.24.0 now implements /string with rank-based cooldowns and persistence. Disable the old StringPlugin JAR so its namespaced command cannot bypass the new cooldown.

Third-party plugins are not rehosted here. Use their official distributions and licenses.

## Combined staff inspection

Install official [AltDetector 1.0.0](https://modrinth.com/plugin/altdetector-plugin) and [ClientPolicy 1.0.0](https://modrinth.com/plugin/clientpolicy), then copy the respective config.yml profiles before starting. AltDetector is All Rights Reserved and its binary is not rehosted here. ClientPolicy retains its MIT license and credits.

Conquest SMP 3.24.0 connects these plugins with GrimAC. Use /conquestac for status, /conquestac inspect <player> for recent source-labelled evidence, /conquestac alts <player> for account links and /conquestac client <player> for online client inspection. Alt auto-bans are disabled and blocked by the bridge; ClientPolicy actions are LOG only. Staff must review matches. Client-announced brands/channels are incomplete and spoofable, and IP matches are not proof of a shared owner or device.

The Conquest evidence store is local, UUID-keyed, capped to the latest 12 results per inspection and retained for 30 days. It does not duplicate raw IPs. AltDetector retains its own local IP history. Do not publish player databases, logs, IP addresses or live credentials.
