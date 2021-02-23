# ssl-game-controller-maven
Distribute the ssl-game-controller via Maven

## Usage with Gradle

```groovy
def osClassifier = {
    def os = System.getProperty("os.name").toLowerCase()
    if (os.contains("windows")) {
        return "windows_amd64"
    } else if (os.contains("linux")) {
        return "linux_amd64"
    } else if (os.contains("mac")) {
        return "darwin_amd64"
    } else {
        throw new IllegalStateException("Unknown operating system: ${os}")
    }
}()

dependencies {
    runtimeOnly "com.github.TIGERs-Mannheim:ssl-game-controller-maven:2.6.2.1:${osClassifier}"
}
```
