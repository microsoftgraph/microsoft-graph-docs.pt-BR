---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 948dcb9ee40730661b6c8221895c88cf1789b6cb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008731"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.TeamsAppsRequestBuilderPostQueryParameters{
    RequiresReview: true,
}
options := &msgraphsdk.TeamsAppsRequestBuilderPostOptions{
    Q: requestParameters,
}
graphClient.AppCatalogs().TeamsApps().Post(options)


```