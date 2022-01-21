---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14fd6d4fad7bcd1b21495e44568f971f8439dab0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137567"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeltaRequestBuilderGetQueryParameters{
    Select: "displayName,jobTitle,mail",
}
options := &msgraphsdk.DeltaRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Contacts().Delta()().Get(options)


```