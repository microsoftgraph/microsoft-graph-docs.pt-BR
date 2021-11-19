---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e510af7c29681eb1f91a98707fcd842926abbd38
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087309"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
outlookTaskId := "outlookTask-id"
result, err := graphClient.UsersById(&userId).Outlook().TasksById(&outlookTaskId).Attachments().Get(options)


```