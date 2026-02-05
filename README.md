# Maestro_Testing_Framework

- Maestro is an open-source framework for mobile and web UI testing 
- GitHub Repository: https://github.com/mobile-dev-inc/maestro 
- Docs: https://docs.maestro.dev/ 

## Setup 

### Prerequisite 
- Maestro requires Java 17 or higher to be installed on your system 
- Run: ```java -version``` to check 

### Installation 

```bash
brew tap mobile-dev-inc/tap 
brew install maestro 
```

### Connection 
- “maestro test” will automatically detect and use any local emulator or USB connected 
Physical Device. 
- Run the Emulator on Android studio, install the QA application on emulator. 

## Studio
- maestro studio is a GUI tool to create and run test flows 
- Run: ```maestro studio``` 

## Flow Creation 
- Start simple in YAML and run it on an emulator or simulator 

```yaml
# flow.yaml 
appId: your.app.id 
--- 
- launchApp 
- tapOn: "Text on the screen" 
```

```yaml
# ex_rupeek.yaml
appId: "com.rupeek.customer.debug" 
--- 
- launchApp 
- assertVisible: "Get Started" 
- tapOn: "Get Started" 
```
- Run: ```maestro test flow.yaml``` 
