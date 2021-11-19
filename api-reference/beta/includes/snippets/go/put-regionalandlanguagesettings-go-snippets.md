---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab3a1645b589eec804fb5e987391a317ca99f098
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096050"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "authoringLanguages":  []Object {
    }
}
options := &msgraphsdk.RegionalAndLanguageSettingsRequestBuilderPutOptions{
    Body: requestBody,
}
graphClient.Me().Settings().RegionalAndLanguageSettings().Put(options)


```