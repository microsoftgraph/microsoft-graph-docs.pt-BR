---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57e6cac34f140449d98bf7c6c94b3256665d5b6d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440209"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDataSource()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.security.siteSource",
}
ediscoveryCaseId := "ediscoveryCase-id"
ediscoverySearchId := "ediscoverySearch-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).SearchesById(&ediscoverySearchId).AdditionalSources().Post(requestBody)


```