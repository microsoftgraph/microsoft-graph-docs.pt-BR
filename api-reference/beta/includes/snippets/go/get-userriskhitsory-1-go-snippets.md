---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e488c6bfa8cf007d22b0e358eba8d73f72254ef8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026399"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

riskyUserId := "riskyUser-id"
result, err := graphClient.RiskyUsersById(&riskyUserId).History().Get(options)


```