---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1cf5edeff488c86b0e7ad34872e6c50080176d38
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757766"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SignInsRequestBuilderGetQueryParameters{
    Filter: "(signInEventTypes/any(t:%20t%20ne%20'interactiveUser'))",
    OrderBy: "createdDateTime%20DESC",
    Top: 10,
}
options := &msgraphsdk.SignInsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AuditLogs().SignIns().Get(options)


```