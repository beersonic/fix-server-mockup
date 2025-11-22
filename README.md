# FIX Server Mockup

This project is a sample FIX acceptor server using QuickFIX/J, built with Gradle.

## Features
- FIXT.1.1/FIX.5.0SP2 support
- Custom session/dictionary configuration
- SLF4J/Log4j2 logging
- Multi-session acceptor

## Usage

### Build
```
./gradlew clean build
```

### Run
```
./gradlew run
```

### Configuration
- Main config: `app/src/main/resources/quickfixj.cfg`
- FIX dictionaries: `app/src/main/resources/FIXT11.xml`, `app/src/main/resources/FIX50SP2.xml`
- Logging: `app/src/main/resources/log4j2.xml`

### Logs
- All runtime logs and FIX message logs are written to the `app/logs/` directory.

## Development
- Java 21 (see `build.gradle`)
- QuickFIX/J 2.3.0
- Gradle wrapper included

## License
MIT
