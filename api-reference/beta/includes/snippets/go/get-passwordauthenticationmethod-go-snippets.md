---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: faa2b9cdcb8a2aa0cb3b449037e98d42927127f4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020631"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

passwordAuthenticationMethodId := "passwordAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().PasswordMethodsById(&passwordAuthenticationMethodId).Get(options)


```