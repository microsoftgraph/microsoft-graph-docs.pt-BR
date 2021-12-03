---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 173835bbe756b48ede9b2082f1e0cf245d019442
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287409"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

eventId := "event-id"
graphClient.Me().EventsById(&eventId).DismissReminder().Post(nil)


```