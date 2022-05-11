---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40b6dde80822d7a09ef6dbcac0c7817b2bfcce09
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323700"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTenantTag()
displayName := "Support"
requestBody.SetDisplayName(&displayName)
description := "Tenants that have purchased extended support"
requestBody.SetDescription(&description)
result, err := graphClient.TenantRelationships().ManagedTenants().TenantTags().Post(requestBody)


```