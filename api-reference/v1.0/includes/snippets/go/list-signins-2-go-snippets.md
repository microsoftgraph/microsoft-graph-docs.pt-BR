---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4887c782d88b86ec77f0357a55e6c3f4ad164c05
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324193"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SignInsRequestBuilderGetQueryParameters{
    Filter: "startsWith(appDisplayName,'Graph')",
    Top: 10,
}
options := &msgraphsdk.SignInsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.AuditLogs().SignIns().GetWithRequestConfigurationAndResponseHandler(options, nil)


```