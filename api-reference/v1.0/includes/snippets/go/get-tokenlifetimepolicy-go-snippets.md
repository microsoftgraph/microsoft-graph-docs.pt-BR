---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a974fdff1d66769be8758ec8e6936acc1c3fd5a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287043"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tokenLifetimePolicyId := "tokenLifetimePolicy-id"
result, err := graphClient.Policies().TokenLifetimePoliciesById(&tokenLifetimePolicyId).Get(nil)


```