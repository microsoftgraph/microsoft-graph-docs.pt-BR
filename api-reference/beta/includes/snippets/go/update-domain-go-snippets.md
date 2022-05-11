---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 194feb8bc9371044e05de6f8045c7b217971f81f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324849"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDomain()
isDefault := true
requestBody.SetIsDefault(&isDefault)
requestBody.SetSupportedServices( []String {
    "Email",
    "OfficeCommunicationsOnline",
}
domainId := "domain-id"
graphClient.DomainsById(&domainId).Patch(requestBody)


```