# ReactNative-Movies
El objetivo de esta sección es crear una aplicación que consuma un **API** de **películas**, para poder construir una aplicación visualmente atractiva y que a la vez nos explique cómo realizar peticiones http y re-utilización de componentes.
Puntualmente:

- Axios
- Custom Hooks aplicados a la realidad
- Loadings
- Promesas simultáneas
- Carousels
- Y más

Esto nos dejará las bases de lo que necesitamos para poder crear aplicaciones con un diseño un poco más complejo en **React
Native**

### Importante
No pude correr en  **iOS** por alguna razon que desconozco, esto despues de agregar lo de los colores. Estuve probando en **Android**
**Log:**
```
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2023-10-12 13:06:36.294 xcodebuild[38100:531600] [MT] DVTAssertions: Warning in /System/Volumes/Data/SWE/Apps/DT/BuildRoots/BuildRoot11/ActiveBuildRoot/Library/Caches/com.apple.xbs/Sources/IDEFrameworks/IDEFrameworks-22267/IDEFoundation/Provisioning/Capabilities Infrastructure/IDECapabilityQuerySelection.swift:103
Details:  createItemModels creation requirements should not create capability item model for a capability item model that already exists.
Function: createItemModels(for:itemModelSource:)
Thread:   <_NSMainThread: 0x600000aa43c0>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
** BUILD FAILED **
```

## Android
![Screenshot_1697138392](https://github.com/manuels-bts/ReactNative-Movies/assets/116088500/373da92a-fa88-4bbc-b5f3-7044b2da5ddb)
![Screenshot_1697138400](https://github.com/manuels-bts/ReactNative-Movies/assets/116088500/3a847b23-e466-4d19-8138-dcd5439bf5a8)
![Screenshot_1697138404](https://github.com/manuels-bts/ReactNative-Movies/assets/116088500/f1d1651c-9d63-4080-a529-a0e28be8a036)

Por alguna razon que desconozco hay un archivo que no se pudo encontrar, Este archivo es sobre colores de los cuales se renderea el Gradiante
```
 ERROR  Error: Cannot find native module 'ImageColors', js engine: hermes
```



