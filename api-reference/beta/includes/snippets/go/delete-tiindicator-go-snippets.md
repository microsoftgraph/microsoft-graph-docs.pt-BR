---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49a90d9d521b7ab545242526af01bc8e65803574
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410883"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tiIndicatorId := "tiIndicator-id"
result, err := graphClient.Security().TiIndicatorsById(&tiIndicatorId).Delete(nil)


```