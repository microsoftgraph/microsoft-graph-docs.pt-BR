---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 512a8894a4a39b8871ed4cf2f5b164800465fdf1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018435"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.OrgContactRequestBuilderGetQueryParameters{
    Select: "displayName,jobTitle,mail",
}
options := &msgraphsdk.OrgContactRequestBuilderGetOptions{
    Q: requestParameters,
}
orgContactId := "orgContact-id"
result, err := graphClient.ContactsById(&orgContactId).Get(options)


```