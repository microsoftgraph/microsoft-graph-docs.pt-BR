---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c03dcb14fd25e35caccf7383778615ae0d5c2713
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322840"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tokenIssuancePolicyId := "tokenIssuancePolicy-id"
result, err := graphClient.Policies().TokenIssuancePoliciesById(&tokenIssuancePolicyId).Get()


```