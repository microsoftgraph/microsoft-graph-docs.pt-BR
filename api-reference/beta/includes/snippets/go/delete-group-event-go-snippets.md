---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d910ae42b959dd1417d810fbfbd900cb3cf3d30d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018657"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
eventId := "event-id"
graphClient.GroupsById(&groupId).EventsById(&eventId).Delete(options)


```