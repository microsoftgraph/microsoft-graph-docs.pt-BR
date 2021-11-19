---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebc0243364a4d155b1210f97bab730ce4e46ab7b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092401"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
softwareOathAuthenticationMethodId := "softwareOathAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().SoftwareOathMethodsById(&softwareOathAuthenticationMethodId).Delete(options)


```