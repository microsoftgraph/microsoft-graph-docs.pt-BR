---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55a515b64e2943a31c5afb2690e7107b15df84a9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323656"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNotebook()
displayName := "My Private notebook"
requestBody.SetDisplayName(&displayName)
result, err := graphClient.Me().Onenote().Notebooks().Post(requestBody)


```