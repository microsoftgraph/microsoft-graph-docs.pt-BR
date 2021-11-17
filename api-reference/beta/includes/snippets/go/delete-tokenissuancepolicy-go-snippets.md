---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f751e5b39ee07958873f5f1b3fc7d9c81c681179
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017335"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

tokenIssuancePolicyId := "tokenIssuancePolicy-id"
graphClient.Policies().TokenIssuancePoliciesById(&tokenIssuancePolicyId).Delete(options)


```