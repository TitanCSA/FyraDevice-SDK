# FyraDevice SDK packages

Public Windows x64 user-mode SDK source packages. These folders contain the existing SDK and its licenses; no kernel driver, activation secret or installer is included.

- [Native SDK source and recipes](https://github.com/TitanCSA/sdk-packages/blob/main/projects/FyraDevice/packaging/native/README.txt)
- [Registry status](SDK-PUBLICATION.md)

Downloadable release artifacts do not imply publication on a central package registry.

<!-- central-sdk-packages:start -->
## Paquets et installation

Les sources, licences, guides API et exemples sont regroupes dans [le depot SDK dedie](https://github.com/TitanCSA/sdk-packages/tree/main/projects/FyraDevice). Choisis le paquet a installer puis execute sa commande dans son dossier.

| Registre | Paquet | Installation / utilisation |
| --- | --- | --- |
| vcpkg | `fyradevice` | `vcpkg install fyradevice:x64-windows` |
| Conan | `fyradevice` | `conan install --requires=fyradevice/0.1.0 -r titancsa --build=missing -s compiler.cppstd=17` |
| NuGet | `FyraDevice.Native` | `Install-Package FyraDevice.Native -Version 0.1.0` |
| NuGet | `FyraDevice.SDK` | `dotnet add package FyraDevice.SDK --version 1.0.0` |
| PyPI | `fyradevice` | Commande prevue apres publication : `python -m pip install fyradevice==1.0.0` |
| Conda | `fyradevice` | `conda install --override-channels -c https://raw.githubusercontent.com/TitanCSA/sdk-packages/089bc73095aa8eda89bacbe10d0b9e58394b0207/conda-channel -c conda-forge fyradevice` (canal TitanCSA) |
| crates.io | `fyradevice` | `cargo add fyradevice@1.0.0` |
| npm | `fyradevice` | Commande prevue apres publication : `npm install fyradevice@1.0.0` |
| Maven Central | `io.github.titancsa:fyradevice` | `io.github.titancsa:fyradevice:1.0.0 (pom.xml / Gradle)` |
| JitPack | `com.github.TitanCSA:FyraDevice-SDK` | `com.github.TitanCSA:FyraDevice-SDK:java-sdk-v1.0.0 (avec le depot JitPack)` |
| Go Modules | `github.com/TitanCSA/FyraDevice-SDK/FyraDevice-Go-modules` | `go get github.com/TitanCSA/FyraDevice-SDK/FyraDevice-Go-modules@v1.0.0` |
| pkg.go.dev | `github.com/TitanCSA/FyraDevice-SDK/FyraDevice-Go-modules` | `Documentation : https://pkg.go.dev/github.com/TitanCSA/FyraDevice-SDK/FyraDevice-Go-modules@v1.0.0` |
| PowerShell Gallery | `fyradevice` | `Install-Module FyraDevice -RequiredVersion 1.0.0 -Scope CurrentUser` |
| pub.dev | `fyradevice` | `dart pub add fyradevice:1.0.0` |
| RubyGems | `fyradevice` | `gem install fyradevice -v 1.0.0` |
| Packagist | `fyradevice` | Commande prevue apres publication : `composer require titancsa/fyradevice:1.0.0` |

Pour vcpkg et Conan, configure d abord le registre TitanCSA avec [le guide complet](https://github.com/TitanCSA/sdk-packages/tree/main/projects/FyraDevice/README.md). Le guide explique aussi Maven/Gradle, les prerequis et le chargement des DLL. Les pilotes/applications du produit sont installes separement. Les commandes marquees prevues ne sont pas encore disponibles.

Les anciens imports Go et versions JitPack gardent leurs tags. Pour les anciennes archives SDK, utilise [les liens de remplacement](https://github.com/TitanCSA/sdk-packages/blob/main/release-assets/URL-MIGRATION.json).
<!-- central-sdk-packages:end -->
