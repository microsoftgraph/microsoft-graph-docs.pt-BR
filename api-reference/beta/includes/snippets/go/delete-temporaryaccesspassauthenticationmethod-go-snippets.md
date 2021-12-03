---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01e856785fbfadfe2b988c3b42e81443269614ad
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286239"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
temporaryAccessPassAuthenticationMethodId := "temporaryAccessPassAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().TemporaryAccessPassMethodsById(&temporaryAccessPassAuthenticationMethodId).Delete(nil)


```