---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8477cc1b0c9095372fb9b6320d248c9f1f888033
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325372"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
outlookTaskId := "outlookTask-id"
result, err := graphClient.UsersById(&userId).Outlook().TasksById(&outlookTaskId).Attachments().Get()


```