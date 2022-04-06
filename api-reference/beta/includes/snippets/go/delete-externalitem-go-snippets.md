---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9f3be7cef9b6fb122e8371f149e35f653cd6891
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63527939"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
externalItemId := "externalItem-id"
graphClient.External().ConnectionsById(&externalConnectionId).ItemsById(&externalItemId).Delete(nil)


```