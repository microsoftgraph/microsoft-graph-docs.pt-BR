---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9a3578ef62e11c25ff4ce51ea3baf950c1fe617
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324020"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationClass()
description := "History - World History 1"
requestBody.SetDescription(&description)
displayName := "World History Level 1"
requestBody.SetDisplayName(&displayName)
educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).Patch(requestBody)


```