---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4f221bd9da4fe7058a9044233458401040ac138d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996880"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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