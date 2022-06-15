---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28cf238fc646fd158695f4bcdcc903a4fd09d094
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092943"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryHoldPolicyId := "ediscoveryHoldPolicy-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).LegalHoldsById(&ediscoveryHoldPolicyId).Get()


```