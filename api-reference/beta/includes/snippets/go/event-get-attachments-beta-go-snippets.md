---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb679484af03e483660d3e894e07360491179a11
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004902"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Attachments().Get(options)


```