---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52637ba1f190cf3cc8f16b397d0ecc01b63d34c1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018672"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewReviewSetQuery()
displayName := "My Query 1"
requestBody.SetDisplayName(&displayName)
query := "(subject:"Quarterly Financials")"
requestBody.SetQuery(&query)
options := &msgraphsdk.QueriesRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
reviewSetId := "reviewSet-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).Queries().Post(options)


```