---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0f5a6071276b85147e0c89a9a5fc96ca03d9888
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287242"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

passwordAuthenticationMethodId := "passwordAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().PasswordMethodsById(&passwordAuthenticationMethodId).Get(nil)


```