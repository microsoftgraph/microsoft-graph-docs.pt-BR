---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5cfcdd91c52527542b0da97386c5508708c35cc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325373"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
microsoftAuthenticatorAuthenticationMethodId := "microsoftAuthenticatorAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().MicrosoftAuthenticatorMethodsById(&microsoftAuthenticatorAuthenticationMethodId).Delete()


```