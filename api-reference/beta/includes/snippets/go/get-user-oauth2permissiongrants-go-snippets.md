---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2c4ff9b24b227bad2b8899c4e99471141559e05
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086771"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Oauth2PermissionGrants().Get(options)


```