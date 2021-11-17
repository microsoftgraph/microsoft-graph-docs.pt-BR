---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3a939e380365554813a0f660c0123e8373eb224
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031021"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

eventId := "event-id"
graphClient.Me().EventsById(&eventId).DismissReminder().Post(options)


```