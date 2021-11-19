---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 248790e47f4fb3169ffaa4b44c74fdf4e71deeaa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085147"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tokenIssuancePolicyId := "tokenIssuancePolicy-id"
result, err := graphClient.Policies().TokenIssuancePoliciesById(&tokenIssuancePolicyId).Get(options)


```