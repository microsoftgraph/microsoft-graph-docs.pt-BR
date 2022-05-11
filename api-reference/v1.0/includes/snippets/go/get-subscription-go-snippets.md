---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0fc9b364bf93e4d3770f710836f1047993b885e5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324189"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

subscriptionId := "subscription-id"
result, err := graphClient.SubscriptionsById(&subscriptionId).Get()


```