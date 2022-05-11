---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afe9601da375b546668f04f0e3f6cbbeb19f76e3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323732"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Oauth2PermissionGrants().Get()


```