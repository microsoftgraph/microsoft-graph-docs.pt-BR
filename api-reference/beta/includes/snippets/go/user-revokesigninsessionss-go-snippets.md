---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abc1e0a86c734060659562302140d556dc0d02bf
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088707"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().RevokeSignInSessions().Post(options)


```