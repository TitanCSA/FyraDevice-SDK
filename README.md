# FyraDevice SDK packages

Public Windows x64 user-mode SDK source packages. These folders contain the existing SDK and its licenses; no kernel driver, activation secret or installer is included.

- [Native SDK source and recipes](https://github.com/TitanCSA/sdk-packages/blob/main/projects/FyraDevice/packaging/native/README.txt)
- [Registry status](SDK-PUBLICATION.md)

Downloadable release artifacts do not imply publication on a central package registry.

<!-- central-sdk-packages:start -->
## SDK : langages et installation

Les sources, licences, guides API et exemples des SDK sont regroupes dans [le depot dedie](https://github.com/TitanCSA/sdk-packages/tree/main/projects/FyraDevice). Choisis ton langage ci-dessous, puis execute sa commande dans le dossier de ton application.

| Langage / registre | Disponibilite | Installation / utilisation |
| --- | --- | --- |
| C++ / vcpkg | Registre TitanCSA disponible (configuration ci-dessous) | `vcpkg install fyradevice:x64-windows` |
| C++ / Conan | Registre TitanCSA disponible (configuration ci-dessous) | `conan install --requires=fyradevice/0.1.0 -r titancsa --build=missing -s compiler.cppstd=17` |
| C++ / NuGet natif | Publie et verifie | `Install-Package FyraDevice.Native -Version 0.1.0` |
| C# / .NET | Publie et verifie | `dotnet add package FyraDevice.SDK --version 1.0.0` |
| Python / pip | Pas encore disponible / validation en cours | Commande prevue apres publication : `python -m pip install fyradevice==1.0.0` |
| Python / Conda | Canal TitanCSA disponible ; acceptation conda-forge encore en attente | `conda install --override-channels -c https://raw.githubusercontent.com/TitanCSA/sdk-packages/089bc73095aa8eda89bacbe10d0b9e58394b0207/conda-channel -c conda-forge fyradevice` |
| Rust / Cargo | Publie et verifie | `cargo add fyradevice@1.0.0` |
| JavaScript et TypeScript / npm | Pas encore disponible / validation en cours | Commande prevue apres publication : `npm install fyradevice@1.0.0` |
| Java et Kotlin / Maven Central | Publie et verifie | `io.github.titancsa:fyradevice:1.0.0 (pom.xml / Gradle)` |
| Java et Kotlin / JitPack | Publie et verifie | `com.github.TitanCSA:FyraDevice-SDK:java-sdk-v1.0.0 (avec le depot JitPack)` |
| Go / Go Modules | Publie et verifie | `go get github.com/TitanCSA/FyraDevice-SDK/FyraDevice-Go-modules@v1.0.0` |
| Go / pkg.go.dev | Publie et verifie | `Documentation : https://pkg.go.dev/github.com/TitanCSA/FyraDevice-SDK/FyraDevice-Go-modules@v1.0.0` |
| PowerShell / Gallery | Publie et verifie | `Install-Module FyraDevice -RequiredVersion 1.0.0 -Scope CurrentUser` |
| Dart et Flutter / pub.dev | Pas encore disponible / validation en cours | Commande prevue apres publication : `dart pub add fyradevice:1.0.0` |
| Ruby / RubyGems | Publie et verifie | `gem install fyradevice -v 1.0.0` |
| PHP / Composer | Pas encore disponible / validation en cours | Commande prevue apres publication : `composer require titancsa/fyradevice:1.0.0` |

Pour vcpkg et Conan, configure d abord le registre TitanCSA avec [ces instructions](https://github.com/TitanCSA/sdk-packages/tree/main/projects/FyraDevice/README.md#c-et-c). Pour Java/Kotlin, le guide donne le bloc Maven/Gradle a ajouter. Windows x64 est requis pour les bindings natifs ; les pilotes/applications restent a installer separement.

Les commandes indiquees comme prevues ne sont pas encore disponibles. Les versions Go/JitPack existantes utilisent les anciens tags conserves ; aucun ancien import Go n est renomme.

[Guide complet, prerequis et exemples](https://github.com/TitanCSA/sdk-packages/tree/main/projects/FyraDevice/README.md).
<!-- central-sdk-packages:end -->
