---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df4461158c78adf034b0ca5cfd1299c5e117c5ca
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985799"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
passwordlessMicrosoftAuthenticatorAuthenticationMethodId := "passwordlessMicrosoftAuthenticatorAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().PasswordlessMicrosoftAuthenticatorMethodsById(&passwordlessMicrosoftAuthenticatorAuthenticationMethodId).Delete(options)


```