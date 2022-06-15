---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6c7cc3d49163aa8e466ac1fb9b3c53acc6b7a8c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096075"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewRegionalAndLanguageSettings()
requestBody.SetAuthoringLanguages( []LocaleInfo {
    msgraphsdk.NewLocaleInfo(),
locale := "en-US"
    SetLocale(&locale)
    msgraphsdk.NewLocaleInfo(),
locale := "es-MX"
    SetLocale(&locale)
}
defaultRegionalFormat := msgraphsdk.NewLocaleInfo()
requestBody.SetDefaultRegionalFormat(defaultRegionalFormat)
locale := "en-US"
defaultRegionalFormat.SetLocale(&locale)
graphClient.Me().Settings().RegionalAndLanguageSettings().Patch(requestBody)


```