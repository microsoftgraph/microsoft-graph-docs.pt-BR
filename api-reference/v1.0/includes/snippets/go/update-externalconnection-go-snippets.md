---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75dde9b000524171d9b2efd23e89f9d34b167a4e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325629"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExternalConnection()
name := "Contoso HR Service Tickets"
requestBody.SetName(&name)
description := "Connection to index HR service tickets"
requestBody.SetDescription(&description)
externalConnectionId := "externalConnection-id"
graphClient.External().ConnectionsById(&externalConnectionId).Patch(requestBody)


```