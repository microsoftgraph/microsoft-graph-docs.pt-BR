---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0f268ca6c516b66505f2e2032e1ebb0ddb05736d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323471"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

eventId := "event-id"
attachmentId := "attachment-id"
graphClient.Me().EventsById(&eventId).AttachmentsById(&attachmentId).Delete()


```