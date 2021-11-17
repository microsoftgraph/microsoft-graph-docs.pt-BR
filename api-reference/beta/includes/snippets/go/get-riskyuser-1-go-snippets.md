---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fca65f7deb3827ef853e9eb561c27b0150fa563b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993891"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

riskyUserId := "riskyUser-id"
result, err := graphClient.RiskyUsersById(&riskyUserId).Get(options)


```