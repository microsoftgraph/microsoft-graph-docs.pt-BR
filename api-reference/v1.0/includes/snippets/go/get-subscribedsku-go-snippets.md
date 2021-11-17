---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 026158f701d1a4b2681e867ab2db44bf577a08cb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003503"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

subscribedSkuId := "subscribedSku-id"
result, err := graphClient.SubscribedSkusById(&subscribedSkuId).Get(options)


```