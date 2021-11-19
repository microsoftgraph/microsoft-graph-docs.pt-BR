---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce430e30a4161f4754db47adbd4cda6c3f86f571
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096971"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

webAccountId := "webAccount-id"
graphClient.Me().Profile().WebAccountsById(&webAccountId).Delete(options)


```