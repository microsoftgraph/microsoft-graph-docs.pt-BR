---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8930860caed298f5344aae38bef2e59f2243a3e
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286147"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcOnPremisesConnectionId := "cloudPcOnPremisesConnection-id"
graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnectionsById(&cloudPcOnPremisesConnectionId).RunHealthChecks().Post(nil)


```