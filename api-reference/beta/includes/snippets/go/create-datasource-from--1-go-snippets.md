---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bed4276dafcd90494dd79cc6db73ef00154de5e9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323119"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDataSource()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.ediscovery.siteSource",
}
caseId := "case-id"
sourceCollectionId := "sourceCollection-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).SourceCollectionsById(&sourceCollectionId).AdditionalSources().Post(requestBody)


```