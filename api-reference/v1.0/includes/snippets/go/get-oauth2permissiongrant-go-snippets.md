---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1125d1a948d51cd3fb969b30b89d75bdd7aaa436
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325102"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

oAuth2PermissionGrantId := "oAuth2PermissionGrant-id"
result, err := graphClient.Oauth2PermissionGrantsById(&oAuth2PermissionGrantId).Get()


```