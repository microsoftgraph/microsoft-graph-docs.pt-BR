---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a5df34a0797aad19377913b861814920ef874c6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985812"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

passwordlessMicrosoftAuthenticatorAuthenticationMethodId := "passwordlessMicrosoftAuthenticatorAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().PasswordlessMicrosoftAuthenticatorMethodsById(&passwordlessMicrosoftAuthenticatorAuthenticationMethodId).Get(options)


```