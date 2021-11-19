---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ace3906384f1bea01b33ca18e572197fdeaaa5d2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100435"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetTagsToAdd( []Tag {
    msgraphsdk.NewTag(),
    SetAdditionalData(map[string]interface{}{
        "id": "b4798d14-748d-468e-a1ec-96a2b1d49677",
    }
}
options := &msgraphsdk.ApplyTagsRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
reviewSetId := "reviewSet-id"
reviewSetQueryId := "reviewSetQuery-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).QueriesById(&reviewSetQueryId).ApplyTags().Post(options)


```