---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d25ae601925d4ffea4c9e2f38599450e13a8115a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323265"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

oAuth2PermissionGrantId := "oAuth2PermissionGrant-id"
graphClient.Oauth2PermissionGrantsById(&oAuth2PermissionGrantId).Delete()


```