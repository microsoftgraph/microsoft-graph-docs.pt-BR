---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9e1d7d4ff7cbb44ba96e2f8356f8480255dd1dcb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325410"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIsSyncedFromOnPremisesRequestBody()
isSyncedFromOnPremises := true
requestBody.SetIsSyncedFromOnPremises(&isSyncedFromOnPremises)
result, err := graphClient.DirectoryObjects().GetAvailableExtensionProperties().Post(requestBody)


```