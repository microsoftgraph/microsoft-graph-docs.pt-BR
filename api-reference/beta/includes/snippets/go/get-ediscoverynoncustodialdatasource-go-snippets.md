---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcdee7dc5a8114f0a2bc61f25621ae554cc918ee
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092130"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EdiscoveryNoncustodialDataSourceRequestBuilderGetQueryParameters{
    Expand: "dataSource",
}
options := &msgraphsdk.EdiscoveryNoncustodialDataSourceRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryNoncustodialDataSourceId := "ediscoveryNoncustodialDataSource-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).NoncustodialDataSourcesById(&ediscoveryNoncustodialDataSourceId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```