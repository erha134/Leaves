Leaves
--------

**English** | [中文](https://github.com/LeavesMC/Leaves/blob/master/README_cn.md)

> Fork of [Paper](https://github.com/PaperMC/Paper) aimed at repairing broken vanilla properties.

> Waring: This fork will have low mspt as Paper

## How To (Server Admins)
Leaves use the same paperclip jar system that Paper uses.

You can download the latest build (1.17.x) of Leaves by going [here](null)

You can also [build it yourself](https://github.com/LeavesMC/Leaves#building).

## How To (Plugin developers)
In order to use Leaves as a dependency you must [build it yourself](https://github.com/LeavesMC/Leaves#building).
Each time you want to update your dependency you must re-build Leaves.

Leaves-API maven dependency:
```xml
<dependency>
    <groupId>top.leavesmc.leaves</groupId>
    <artifactId>leaves-api</artifactId>
    <version>1.17.1-R0.1-SNAPSHOT</version>
    <scope>provided</scope>
 </dependency>
 ```

Leaves-Server maven dependency:
```xml
<dependency>
    <groupId>top.leavesmc.leaves</groupId>
    <artifactId>leaves</artifactId>
    <version>1.17.1-R0.1-SNAPSHOT</version>
    <scope>provided</scope>
</dependency>
```

## Building
Java16+

`./gradlew applyPatches`

`./gradlew build`

`./gradlew paperclipJar` or `./gradlew reobfJar`