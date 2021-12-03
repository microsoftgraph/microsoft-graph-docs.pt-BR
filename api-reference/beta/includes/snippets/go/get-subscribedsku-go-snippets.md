---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2be215f6bba844c127afbeb1712fadeddc42808
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286729"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

subscribedSkuId := "subscribedSku-id"
result, err := graphClient.SubscribedSkusById(&subscribedSkuId).Get(nil)


```