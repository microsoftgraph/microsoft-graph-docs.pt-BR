---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7beef224fe15d5e9b2ba8418d162df92ef9b73e
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62530482"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ContactsRequestBuilderGetQueryParameters{
    Filter: "startswith(displayName,'A')",
    Count: true,
    Top: 1,
    Orderby: "displayName",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.ContactsRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Contacts().Get(options)


```