---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01b044c48f6614c834c7be1c90a4b80c242ae739
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033346"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UserScopeTeamsAppInstallationRequestBuilderGetQueryParameters{
    Expand: "teamsAppDefinition",
}
options := &msgraphsdk.UserScopeTeamsAppInstallationRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
userScopeTeamsAppInstallationId := "userScopeTeamsAppInstallation-id"
result, err := graphClient.UsersById(&userId).Teamwork().InstalledAppsById(&userScopeTeamsAppInstallationId).Get(options)


```