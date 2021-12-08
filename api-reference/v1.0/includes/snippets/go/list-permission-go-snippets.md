---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a22d4f90b19d025848f8f63dddcf3d4baa41c1b7
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348755"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SitesRequestBuilderGetQueryParameters{
    Search: "%7Bquery%7D",
}
options := &msgraphsdk.SitesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Sites().Get(options)


```