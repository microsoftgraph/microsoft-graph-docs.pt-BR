---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 281bee6cf0a27438d82d9c89e21c2c7b0884f830
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60999519"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

calendarGroupId := "calendarGroup-id"
result, err := graphClient.Me().CalendarGroupsById(&calendarGroupId).Calendars().Get(options)


```