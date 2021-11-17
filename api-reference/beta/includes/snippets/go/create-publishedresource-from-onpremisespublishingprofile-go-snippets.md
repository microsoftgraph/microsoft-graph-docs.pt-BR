---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfb7812da8dde7ba66b6147917541fb2b96d6654
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004455"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPublishedResource()
displayName := "New provisioning"
requestBody.SetDisplayName(&displayName)
resourceName := "domain1.contoso.com"
requestBody.SetResourceName(&resourceName)
options := &msgraphsdk.PublishedResourcesRequestBuilderPostOptions{
    Body: requestBody,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).PublishedResources().Post(options)


```