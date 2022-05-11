---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26ec7f92afe74ca0df2b57ea8bdbebb73db44433
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324856"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCrossTenantAccessPolicy()
displayName := "CrossTenantAccessPolicy"
requestBody.SetDisplayName(&displayName)
graphClient.Policies().CrossTenantAccessPolicy().Patch(requestBody)


```