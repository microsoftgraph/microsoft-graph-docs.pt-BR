---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d93ad8bc42d73822a3f9bd47c26b91cc02ed1d02
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322967"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
allowedToUseSSPR := true
requestBody.SetAllowedToUseSSPR(&allowedToUseSSPR)
graphClient.Policies().AuthorizationPolicy().Patch(requestBody)


```