---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee257442945dc02578ebd553dd070e61989f406e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322237"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOAuth2PermissionGrant()
scope := "User.ReadBasic.All Group.ReadWrite.All"
requestBody.SetScope(&scope)
oAuth2PermissionGrantId := "oAuth2PermissionGrant-id"
graphClient.Oauth2PermissionGrantsById(&oAuth2PermissionGrantId).Patch(requestBody)


```