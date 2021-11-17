---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d1ab2dca41955d4e4e40bd7745c2113c2d1bea7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61000933"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

calendarGroupId := "calendarGroup-id"
graphClient.Me().CalendarGroupsById(&calendarGroupId).Delete(options)


```