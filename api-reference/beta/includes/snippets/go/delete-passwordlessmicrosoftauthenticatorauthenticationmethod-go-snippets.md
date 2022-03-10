---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f01d26c9a827ea5570f039590fb0e44b8e218dd0
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411405"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
passwordlessMicrosoftAuthenticatorAuthenticationMethodId := "passwordlessMicrosoftAuthenticatorAuthenticationMethod-id"
result, err := graphClient.UsersById(&userId).Authentication().PasswordlessMicrosoftAuthenticatorMethodsById(&passwordlessMicrosoftAuthenticatorAuthenticationMethodId).Delete(nil)


```