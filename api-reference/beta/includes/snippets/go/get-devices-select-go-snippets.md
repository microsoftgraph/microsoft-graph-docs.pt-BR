---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e99aa759e9f4d126a56ba437b8ac089d17f09b67
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005385"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.DevicesRequestBuilderGetQueryParameters{
    Select: "id,extensionAttributes",
}
options := &msgraphsdk.DevicesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Devices().Get(options)


```