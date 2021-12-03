---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c1a0eac92786150b9715e979d5494cd7054462b
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286641"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tokenLifetimePolicyId := "tokenLifetimePolicy-id"
graphClient.Policies().TokenLifetimePoliciesById(&tokenLifetimePolicyId).Delete(nil)


```