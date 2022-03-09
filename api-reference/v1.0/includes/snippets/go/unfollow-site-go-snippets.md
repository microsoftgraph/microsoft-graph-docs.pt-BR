---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3290434ef581f6d229c0f9c4176cbdd7225b019
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393175"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "value":  []Object {
    }
}
options := &msgraphsdk.SiteRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
siteId := "site-id"
graphClient.UsersById(&userId).FollowedSitesById(&siteId).Post(options)


```