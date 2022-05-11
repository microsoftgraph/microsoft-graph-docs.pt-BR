---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54c164f54299f6265fbd27cf622cea579f5de6b8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323064"
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
result, err := graphClient.Directory().AdministrativeUnits().Post(requestBody)


```