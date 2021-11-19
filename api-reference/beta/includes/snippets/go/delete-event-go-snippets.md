---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69fe45f5515fc05a0d9fbed22ffed71514fff44b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099026"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

eventId := "event-id"
graphClient.Me().EventsById(&eventId).Delete(options)


```