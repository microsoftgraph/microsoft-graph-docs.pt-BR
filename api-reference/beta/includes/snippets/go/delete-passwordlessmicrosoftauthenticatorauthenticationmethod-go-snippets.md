---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 590ca085b3274bab79e0918ca7b98bdf066ec32b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324330"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
passwordlessMicrosoftAuthenticatorAuthenticationMethodId := "passwordlessMicrosoftAuthenticatorAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().PasswordlessMicrosoftAuthenticatorMethodsById(&passwordlessMicrosoftAuthenticatorAuthenticationMethodId).Delete()


```