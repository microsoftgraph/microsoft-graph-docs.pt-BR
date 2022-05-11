---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a83b0307197b82296e7e918f4b8d049951fc9914
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323764"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentity()
id := "1431b9c38ee647f6a"
requestBody.SetId(&id)
type := "externalGroup"
requestBody.SetType(&type)
externalConnectionId := "externalConnection-id"
externalGroupId := "externalGroup-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).GroupsById(&externalGroupId).Members().Post(requestBody)


```