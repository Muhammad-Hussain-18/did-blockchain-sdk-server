# Server Blockchain SDK
Welcome to the Server Blockchain SDK Repository.
This repository provides an SDK for interacting with Blockchain networks and invoking Smart Contracts.

## Folder Structure
```
did-blockchain-sdk-server
├── CHANGELOG.md
├── CLA.md
├── CODE_OF_CONDUCT.md
├── LICENSE.dependencies.md
├── LICENSE.txt
├── CONTRIBUTING.md
├── MAINTAINERS.md
├── README.md
├── README_ko.md
├── RELEASE-PROCESS.md
├── SECURITY.md
├── docs
│   └── api
│       ├── Blockchain_API.md 
│       ├── Blockchain_API_ko.md 
│       └── BlockchainErrorCode.md 
└── source
    └── did-blockchain-sdk-server
        ├── README.md
        ├── README_ko.md
        ├── build.gradle
        ├── gradle
        ├── gradlew
        ├── gradlew.bat
        ├── setting.gradle
        └── src
```


|  Name                      |              Description                        |
| -------------------------- | ------------------------------------------------|
| CHANGELOG.md               | Version-specific changes in the project         |
| CLA.md                     | Contributor License Agreement                   |
| CODE_OF_CONDUCT.md         | Code of conduct for contributors                |
| CONTRIBUTING.md            | Contribution guidelines and procedures          |
| LICENSE.dependencies.md    | Licenses for the project’s dependency libraries |
| LICENSE.txt                | License for the project                         |
| MAINTAINERS.md             | General guidelines for maintaining              |
| README.md                  | Overview and description of the project         |
| RELEASE-PROCESS.md         | Release process                                 |
| SECURITY.md                | Security policy and vulnerability reporting     | 
| docs                       | Documentation                                   |
| ┖ api                      | API guide documentation                         |
| source                     | SDK source code project                         |

<br>

## Libraries
Libraries can be found in the `release` folder.
1. Copy the `did-datamodel-server-1.0.0.jar` file into the project's `libs` directory.
2. Add the following dependencies to the project's `build.gradle` file:
```groovy
    implementation files('libs/did-datamodel-server-1.0.0.jar')
    implementation('org.hyperledger.fabric:fabric-gateway-java:2.2.9')
    implementation('com.fasterxml.jackson.core:jackson-databind:2.15.2')
    implementation('org.apache.commons:commons-pool2:2.12.0')
    testImplementation platform('org.junit:junit-bom:5.10.0')
    testImplementation('org.junit.jupiter:junit-jupiter')
    annotationProcessor('com.fasterxml.jackson.core:jackson-databind:2.15.2')
    annotationProcessor('org.projectlombok:lombok:1.18.28')
    compileOnly('org.projectlombok:lombok:1.18.28')
```
3. Synchronize `Gradle` to ensure that the dependencies are correctly added.

## API Reference

You can find the API reference [here](source/did-blockchain-sdk-server/README.md).

## Contributing

For detailed information on contributing and submitting pull requests, please refer to [CONTRIBUTING.md](CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).

## License
Copyright 2024 Raonsecure