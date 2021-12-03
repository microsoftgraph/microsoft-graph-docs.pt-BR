---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0480968593ee30454d2abc2685bd2eb18a38c7c5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286858"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

webAccountId := "webAccount-id"
result, err := graphClient.Me().Profile().WebAccountsById(&webAccountId).Get(nil)


```