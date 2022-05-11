---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5a9b9e4a5ec87c9e4882f747f3a4844bcca40577
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324349"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSecurityEnabledOnlyRequestBody()
securityEnabledOnly := true
requestBody.SetSecurityEnabledOnly(&securityEnabledOnly)
result, err := graphClient.Me().GetMemberGroups().Post(requestBody)


```