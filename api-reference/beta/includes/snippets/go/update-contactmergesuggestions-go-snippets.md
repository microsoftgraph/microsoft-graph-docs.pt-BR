---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b720addfc45f6358c6ad7b27b6a695ab1c7f840
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325048"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContactMergeSuggestions()
isEnabled := false
requestBody.SetIsEnabled(&isEnabled)
graphClient.Me().Settings().ContactMergeSuggestions().Patch(requestBody)


```