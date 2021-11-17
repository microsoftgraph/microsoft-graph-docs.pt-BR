---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 312fdcf1fe735e12151cce20d31b9aad061c6705
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031753"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
softwareOathAuthenticationMethodId := "softwareOathAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().SoftwareOathMethodsById(&softwareOathAuthenticationMethodId).Delete(options)


```