---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 321375271439c13c193e0c90a107138ed44dfede
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324456"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "value":  []Object {
    }
}
userId := "user-id"
siteId := "site-id"
graphClient.UsersById(&userId).FollowedSitesById(&siteId).Post(requestBody)


```