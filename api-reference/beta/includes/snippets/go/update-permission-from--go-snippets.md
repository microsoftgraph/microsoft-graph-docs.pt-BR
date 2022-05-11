---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25ff3506520c029d5d5089c56d90eacc0cec32f6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323441"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPermission()
requestBody.SetRoles( []String {
    "read",
}
siteId := "site-id"
permissionId := "permission-id"
graphClient.SitesById(&siteId).PermissionsById(&permissionId).Patch(requestBody)


```