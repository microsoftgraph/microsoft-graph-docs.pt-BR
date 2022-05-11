---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd567af8bf1c73531805fd0142677dc41000dcf1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324327"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonAnnualEvent()
allowedAudiences := "contacts"
requestBody.SetAllowedAudiences(&allowedAudiences)
personAnnualEventId := "personAnnualEvent-id"
graphClient.Me().Profile().AnniversariesById(&personAnnualEventId).Patch(requestBody)


```