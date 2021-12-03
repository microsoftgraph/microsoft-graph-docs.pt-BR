---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7221a5ea77b5dbde7080864278e025ca5d2d8a7a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287431"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

subscriptionId := "subscription-id"
result, err := graphClient.SubscriptionsById(&subscriptionId).Get(nil)


```