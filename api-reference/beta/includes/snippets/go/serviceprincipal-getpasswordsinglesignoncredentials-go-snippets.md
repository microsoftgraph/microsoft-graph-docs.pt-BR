---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95683ed99c215d78dcb5df027aeef223701b10f8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325233"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdRequestBody()
id := "5793aa3b-cca9-4794-679a240f8b58"
requestBody.SetId(&id)
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).GetPasswordSingleSignOnCredentials(servicePrincipal-id).Post(requestBody)


```