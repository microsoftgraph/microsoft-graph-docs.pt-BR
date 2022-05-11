---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae1f1fcd3e814753c2ff0b276a959d620b022bb1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324163"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
userScopeTeamsAppInstallationId := "userScopeTeamsAppInstallation-id"
result, err := graphClient.UsersById(&userId).Teamwork().InstalledAppsById(&userScopeTeamsAppInstallationId).Chat().Get()


```