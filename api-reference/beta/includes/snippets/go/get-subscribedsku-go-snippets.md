---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9694d205ac2ff542a719f457b4dbe2983d545c1f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322991"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

subscribedSkuId := "subscribedSku-id"
result, err := graphClient.SubscribedSkusById(&subscribedSkuId).Get()


```