---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9731df28f6c3cdbdf5ff30cf1dd36e551233414
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323763"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentity()
id := "e5477431-1038-484e-bf69-1dfedb97a110"
requestBody.SetId(&id)
type := "group"
requestBody.SetType(&type)
externalConnectionId := "externalConnection-id"
externalGroupId := "externalGroup-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).GroupsById(&externalGroupId).Members().Post(requestBody)


```