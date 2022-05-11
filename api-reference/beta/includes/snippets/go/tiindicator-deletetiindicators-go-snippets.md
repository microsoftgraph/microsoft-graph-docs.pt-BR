---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0cd2a035e9adf7d04670f137c7c22400b878fb7b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324565"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewValueRequestBody()
requestBody.SetValue( []String {
    "id-value1",
    "id-value2",
}
result, err := graphClient.Security().TiIndicators().DeleteTiIndicators().Post(requestBody)


```