---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e84034e5b0eaf7ca18d92f6d107f302a9f5a2be
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225501"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AttributeSetsRequestBuilderGetQueryParameters{
    OrderBy: "id",
}
options := &msgraphsdk.AttributeSetsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Directory().AttributeSets().Get(options)


```