---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dda5ab6008ea32eaa4d470b5fb8f88cd53417b6f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033793"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9",
}
options := &msgraphsdk.HomeRealmDiscoveryPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).HomeRealmDiscoveryPolicies().Post(options)


```