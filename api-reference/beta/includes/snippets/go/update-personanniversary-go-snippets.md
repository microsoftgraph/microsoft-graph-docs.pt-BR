---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ae5a28f835d6bb3caeb712ebb8357fd87112ec4
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411096"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonAnnualEvent()
allowedAudiences := "contacts"
requestBody.SetAllowedAudiences(&allowedAudiences)
options := &msgraphsdk.PersonAnnualEventRequestBuilderPatchOptions{
    Body: requestBody,
}
personAnnualEventId := "personAnnualEvent-id"
result, err := graphClient.Me().Profile().AnniversariesById(&personAnnualEventId).Patch(options)


```