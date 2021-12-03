---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a72398735350c069cb1c893e2d466d3e4f31559d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287410"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Attachments().Get(nil)


```