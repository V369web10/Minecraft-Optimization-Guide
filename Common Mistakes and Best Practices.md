# 🛠 Common Mistakes and Best Practices

This article aims to explain the most common mistakes and practices related to Minecraft server performance.

## Always **Make a Backup**

It is only a matter of time before we experience data loss. We always make copies to avoid losing our worlds or plugin data. We can apply this to any computer-related workflow, not just Minecraft.

## Avoid Using Outdated Software

If we use outdated software versions, we run the risk of our players abusing unpatched exploits, including item duplication (infinite items). It also adds an inconvenience factor since our players specifically have to downgrade their client version to match our server. This can be prevented by using a protocol hack, but it is not ideal.

## Do Not Run Bukkit/Spigot Anymore

Bukkit and Spigot are basically in maintenance mode. They are updated whenever there is a new version and if a critical exploit is found, but they do not add any performance updates. This means that any performance issues we may experience on those software versions will never improve over time.

To avoid this, use [Paper](https://papermc.io/downloads) or [Purpur](https://purpurmc.org/downloads). Bukkit/Spigot plugins will work just as well (perhaps even better) with the aforementioned server software. If they don't, then it is safe to assume the plugin developer is doing things they shouldn't or did a negligent job creating their plugin. These optimized servers also add optimization patches like a chunk loading system that can take advantage of multiple CPU threads or a setting that allows the server to mark fewer chunks than it actually sends to the player.

## Avoid Shared Hosting if Possible

Shared hosting is usually the cheapest option, and that is for a valid reason. They offer us 2 types of resources – guaranteed and shared. Guaranteed resources are often ridiculously low and may not be enough to run a server for just a few players. On the other hand, shared resources are often sufficient to run a server with decent performance.

Shared resources, as the name suggests, are shared between our server and other servers on the same physical machine. Our server can only benefit from having them when no other server is using them. The situation where our server fully utilizes the shared resources is practically impossible, as most shared hosts oversell their resources. Much like airline tickets, the hosting site sells more resources than it has available in the hope that not all of them will be used. This often leads to situations where all servers are stuck because there are not enough resources to spare.

## Avoid Datapacks that Use Command Functions

Datapacks that execute commands are extremely slow. It might not be much with few players, but that does not scale well with the number of players and will cause your server to slow down quickly as you gain players. Datapacks that modify biomes, loot tables, etc., are fine. However, it is better to look for an alternative plugin.

## Storage Type

We must absolutely avoid Hard Disk Drives (HDDs). Their speeds are simply too slow to justify running a server on, as Minecraft is heavy on I/O operations (especially with high view distances and a higher number of players). A Solid State Drive (SSD) is a much better choice due to its much faster I/O speed.
