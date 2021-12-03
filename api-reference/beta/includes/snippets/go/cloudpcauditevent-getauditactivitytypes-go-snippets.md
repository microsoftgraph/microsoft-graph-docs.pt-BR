---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b88af012d7abbc5dfd34251213950721e46cd7d7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286154"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcAuditEventId := "cloudPcAuditEvent-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().AuditEventsById(&cloudPcAuditEventId).Get(nil)


```