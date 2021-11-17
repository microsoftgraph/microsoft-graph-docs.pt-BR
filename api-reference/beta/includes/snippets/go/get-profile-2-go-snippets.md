---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8be8652acffb4f4da3ded87a0760c86ada73df90
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019554"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ProfileRequestBuilderGetQueryParameters{
    Expand: "names($select=first,last),skills($select=displayName)",
}
options := &msgraphsdk.ProfileRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Profile().Get(options)


```