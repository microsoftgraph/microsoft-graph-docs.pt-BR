---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcbadeb499890317d6e4d1c6d3345256d457ad19
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61013066"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ServiceHealthRequestBuilderGetQueryParameters{
    Expand: "issues",
}
options := &msgraphsdk.ServiceHealthRequestBuilderGetOptions{
    Q: requestParameters,
}
serviceHealthId := "serviceHealth-id"
result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviewsById(&serviceHealthId).Get(options)


```