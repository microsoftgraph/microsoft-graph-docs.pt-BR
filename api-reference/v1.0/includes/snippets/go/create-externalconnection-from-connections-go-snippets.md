---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a8ba0305d7e42aa789f606f9681f660f99e5240
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322427"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExternalConnection()
id := "contosohr"
requestBody.SetId(&id)
name := "Contoso HR"
requestBody.SetName(&name)
description := "Connection to index Contoso HR system"
requestBody.SetDescription(&description)
result, err := graphClient.External().Connections().Post(requestBody)


```