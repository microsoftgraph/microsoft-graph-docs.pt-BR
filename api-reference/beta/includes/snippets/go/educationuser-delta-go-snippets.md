---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8555b263d0f702cab5a645dcd650411935f828b1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990244"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationUserId := "educationUser-id"
result, err := graphClient.Education().UsersById(&educationUserId).Get(options)


```