---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 020e36bdccb12a76037ac73f54d6e1c255a74435
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026539"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
outlookTaskId := "outlookTask-id"
result, err := graphClient.UsersById(&userId).Outlook().TasksById(&outlookTaskId).Attachments().Get(options)


```