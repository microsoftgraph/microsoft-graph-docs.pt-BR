---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2cbaea35192c9d99b20ea6f7daf46faf18ac978a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033381"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.MessagesRequestBuilderGetQueryParameters{
    Select: "sender,subject",
}
options := &msgraphsdk.MessagesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Messages().Get(options)


```