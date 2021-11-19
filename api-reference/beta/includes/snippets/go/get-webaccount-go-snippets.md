---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 248e8f33da4f887e97a051cbbfb7b858dc90b136
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087787"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

webAccountId := "webAccount-id"
result, err := graphClient.Me().Profile().WebAccountsById(&webAccountId).Get(options)


```