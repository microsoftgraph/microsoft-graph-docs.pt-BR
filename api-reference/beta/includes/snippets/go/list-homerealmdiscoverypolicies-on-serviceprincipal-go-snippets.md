---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5027727a38605bc3c800a7220a2afa98db95de96
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977929"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).HomeRealmDiscoveryPolicies().Get(options)


```