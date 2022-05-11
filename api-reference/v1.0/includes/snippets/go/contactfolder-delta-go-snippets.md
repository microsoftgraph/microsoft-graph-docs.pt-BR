---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e075fc23bd3d10de063811957271085b2529dc90
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322670"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "odata.maxpagesize=2"
}
options := &msgraphsdk.DeltaRequestBuilderGetRequestConfiguration{
    Headers: headers,
}
result, err := graphClient.Me().ContactFolders().Delta()().GetWithRequestConfigurationAndResponseHandler(options, nil)


```