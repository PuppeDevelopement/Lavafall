Lavafall
========

Lavafall is a fork of Waterfall, which in turn is based on BungeeCord. This project is maintained with a focus on creating a straightforward, stable server proxy while integrating a few practical improvements.

-------------

How to Use Lavafall (for Server Administrators)
------------------------------------------------
1. **Download Lavafall.jar**  
   You can download the latest jar from our download page:  
   [Lavafall Downloads](https://soon.com).

2. **Requirements**  
   Lavafall requires Java 8 or above.

3. **Setup**  
   Use Lavafall in place of your current proxy setup following your standard installation procedures.

How to Use Lavafall (for Plugin Developers)
--------------------------------------------
For plugin development, Lavafall exposes a public API that can be integrated using Maven or Gradle.

**Maven Setup**  

Add the following repository:

```xml
<repository>
    <id>papermc</id>
    <url>https://repo.papermc.io/repository/maven-public/</url>
</repository>
```

And include the dependency:

```xml
<dependency>
    <groupId>io.github.waterfallmc</groupId>
    <artifactId>waterfall-api</artifactId>
    <version>1.20-R0.1-SNAPSHOT</version>
    <scope>provided</scope>
</dependency>
```

**Gradle Setup**  

Include the repository:

```groovy
repositories {
    maven {
        url 'https://repo.papermc.io/repository/maven-public/'
    }
}
```

And add the dependency:

```groovy
dependencies {
    compileOnly 'io.github.waterfallmc:waterfall-api:1.20-R0.1-SNAPSHOT'
}
```

Compiling from Source
---------------------
To compile Lavafall from source, ensure you have JDK 8 (or later), git, bash, and Maven installed.

1. Clone the repository.
2. Run the build script using:
   ```bash
   ./waterfall build
   ```
3. The compiled jar will be located at `Lavafall-Proxy/bootstrap/target/` after the build completes.

Joining the Community
---------------------
Contributions are welcome. If you’d like to help improve Lavafall, please feel free to open a pull request. You can also join discussions on our [Discord](https://discord.gg/).

Special Thanks
--------------
For all Lavafall developers we want to say special thanks. Thank you for keeping this project going!
