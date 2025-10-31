# SSL Game Controller Maven Package

[![JitPack](https://jitpack.io/v/lkhcode/ssl-game-controller-maven.svg)](https://jitpack.io/#lkhcode/ssl-game-controller-maven)

这个项目将 [lkhcode/ssl-game-controller](https://github.com/lkhcode/ssl-game-controller) 的二进制文件打包为 Maven artifacts，方便在其他 Java/Gradle 项目中使用。

## 使用方法 (通过 JitPack)

### 在 Gradle 项目中使用

1. 在 `build.gradle` 或 `settings.gradle` 中添加 JitPack 仓库：

```gradle
repositories {
    maven { url 'https://jitpack.io' }
}
```

2. 添加依赖：

```gradle
dependencies {
    implementation 'com.github.lkhcode:ssl-game-controller-maven:v0.0.1'
}
```

### 在 Maven 项目中使用

1. 在 `pom.xml` 中添加 JitPack 仓库：

```xml
<repositories>
    <repository>
        <id>jitpack.io</id>
        <url>https://jitpack.io</url>
    </repository>
</repositories>
```

2. 添加依赖：

```xml
<dependency>
    <groupId>com.github.lkhcode</groupId>
    <artifactId>ssl-game-controller-maven</artifactId>
    <version>v0.0.1</version>
</dependency>
```

## 构建状态



## 开发

本地构建：

```bash
./gradlew build publishToMavenLocal
```
