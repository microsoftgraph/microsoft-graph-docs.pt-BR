---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 673bfdb6d3a7c6fb788be2a84206f67f4ab9ccae
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324522"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

homeRealmDiscoveryPolicyId := "homeRealmDiscoveryPolicy-id"
result, err := graphClient.Policies().HomeRealmDiscoveryPoliciesById(&homeRealmDiscoveryPolicyId).Get()


```