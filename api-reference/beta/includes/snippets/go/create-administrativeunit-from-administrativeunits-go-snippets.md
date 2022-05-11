---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84b6bb33ffe8618c396a4d07edbdafcf833095ab
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324852"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAdministrativeUnit()
displayName := "Seattle District Technical Schools"
requestBody.SetDisplayName(&displayName)
description := "Seattle district technical schools administration"
requestBody.SetDescription(&description)
visibility := "HiddenMembership"
requestBody.SetVisibility(&visibility)
result, err := graphClient.AdministrativeUnits().Post(requestBody)


```