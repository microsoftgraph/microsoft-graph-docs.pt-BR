---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d52d49cb14edaa7bb8a746a8c31725c87cfdc8e6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323591"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageCatalog()
displayName := "sales"
requestBody.SetDisplayName(&displayName)
description := "for employees working with sales and outside sales partners"
requestBody.SetDescription(&description)
state := "published"
requestBody.SetState(&state)
isExternallyVisible := true
requestBody.SetIsExternallyVisible(&isExternallyVisible)
result, err := graphClient.IdentityGovernance().EntitlementManagement().Catalogs().Post(requestBody)


```