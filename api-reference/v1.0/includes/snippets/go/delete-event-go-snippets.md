---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48ae9fae04c04aee8400b16b87ee229a697a6157
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411310"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Delete(nil)


```