---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74dcaf5c09b0c5a2d6d47eb050b22cd5c9d9187c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325371"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewWebUrlRequestBody()
webUrl := "webUrl value"
requestBody.SetWebUrl(&webUrl)
result, err := graphClient.Me().Onenote().Notebooks().GetNotebookFromWebUrl().Post(requestBody)


```