---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 501aac0102dd585ad992729ed944f45b5978f11f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985252"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ContactsRequestBuilderGetQueryParameters{
    Select: "displayName,emailAddresses",
}
options := &msgraphsdk.ContactsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Contacts().Get(options)


```