---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9bd38e76602f8fc98a296b5aced5eee6649abd2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005036"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
emailAuthenticationMethodId := "emailAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().EmailMethodsById(&emailAuthenticationMethodId).Delete(options)


```