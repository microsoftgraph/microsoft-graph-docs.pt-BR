---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef9282aa5ea3429d00155302207d20ead391aedb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022354"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewReviewSetQuery()
displayName := "My Query 1 - Renamed"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ReviewSetQueryRequestBuilderPatchOptions{
    Body: requestBody,
}
caseId := "case-id"
reviewSetId := "reviewSet-id"
reviewSetQueryId := "reviewSetQuery-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).QueriesById(&reviewSetQueryId).Patch(options)


```