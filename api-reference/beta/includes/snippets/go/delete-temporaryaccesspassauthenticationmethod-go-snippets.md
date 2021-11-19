---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d859b3f91471713b7826ef16f7d79cfffa576b71
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097261"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
temporaryAccessPassAuthenticationMethodId := "temporaryAccessPassAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().TemporaryAccessPassMethodsById(&temporaryAccessPassAuthenticationMethodId).Delete(options)


```