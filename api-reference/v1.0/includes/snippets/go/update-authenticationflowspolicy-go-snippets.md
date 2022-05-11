---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1cf2e4ae290cba415b2bda72173fa122f921a6dc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323404"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthenticationFlowsPolicy()
selfServiceSignUp := msgraphsdk.NewSelfServiceSignUpAuthenticationFlowConfiguration()
requestBody.SetSelfServiceSignUp(selfServiceSignUp)
isEnabled := true
selfServiceSignUp.SetIsEnabled(&isEnabled)
graphClient.Policies().AuthenticationFlowsPolicy().Patch(requestBody)


```