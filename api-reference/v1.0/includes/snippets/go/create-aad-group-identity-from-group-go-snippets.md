---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c9588af4fd52c54f866179dfb3a269f0d08ab3a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394961"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentity()
id := "e5477431-1038-484e-bf69-1dfedb97a110"
requestBody.SetId(&id)
type := "group"
requestBody.SetType(&type)
options := &msgraphsdk.MembersRequestBuilderPostOptions{
    Body: requestBody,
}
externalConnectionId := "externalConnection-id"
externalGroupId := "externalGroup-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).GroupsById(&externalGroupId).Members().Post(options)


```