---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7607881af9cfda537f4e651261b9859ddcc02cd1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002641"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.SchemaExtensionsRequestBuilderGetQueryParameters{
    Filter: "id%20eq%20'graphlearn_test'",
}
options := &msgraphsdk.SchemaExtensionsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.SchemaExtensions().Get(options)


```