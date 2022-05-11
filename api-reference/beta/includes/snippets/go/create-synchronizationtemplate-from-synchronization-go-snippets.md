---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f86b33e4dab96a612017a334866cb1e9eadd303
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323438"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSynchronizationTemplate()
id := "SCIM-Test1"
requestBody.SetId(&id)
applicationId := "{id}"
requestBody.SetApplicationId(&applicationId)
factoryTag := "CustomSCIM"
requestBody.SetFactoryTag(&factoryTag)
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).Synchronization().Templates().Post(requestBody)


```