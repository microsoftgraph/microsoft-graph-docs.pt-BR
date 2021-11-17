---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5537c4ae8d5e5c7e82fb45ce0f5ebd6847a35f0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994381"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.SourceCollectionRequestBuilderGetQueryParameters{
    Expand: "addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation",
}
options := &msgraphsdk.SourceCollectionRequestBuilderGetOptions{
    Q: requestParameters,
}
caseId := "case-id"
sourceCollectionId := "sourceCollection-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).SourceCollectionsById(&sourceCollectionId).Get(options)


```