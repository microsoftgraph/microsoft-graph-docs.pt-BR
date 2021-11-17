---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18d6640a07d6f2470b011089053b5a8ae8ec3972
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985694"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPersonAnnualEvent()
allowedAudiences := "contacts"
requestBody.SetAllowedAudiences(&allowedAudiences)
options := &msgraphsdk.PersonAnnualEventRequestBuilderPatchOptions{
    Body: requestBody,
}
personAnnualEventId := "personAnnualEvent-id"
graphClient.Me().Profile().AnniversariesById(&personAnnualEventId).Patch(options)


```