---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abe7258bd2429c75f0d4da3b610a2937b661a5c0
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411276"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

eventId := "event-id"
graphClient.Me().EventsById(&eventId).DismissReminder(event-id).Post(nil)


```