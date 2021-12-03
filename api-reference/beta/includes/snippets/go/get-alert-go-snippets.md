---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 577bcda4d69b5f64656e0c4090b62a962aad8858
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285876"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

alertId := "alert-id"
result, err := graphClient.Security().AlertsById(&alertId).Get(nil)


```