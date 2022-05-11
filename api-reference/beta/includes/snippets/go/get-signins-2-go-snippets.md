---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8179a46136a4cc48449d5aef716710fded7f4bb9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324388"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SignInsRequestBuilderGetQueryParameters{
    Filter: "startsWith(appDisplayName,'Azure')",
    Top: 10,
}
options := &msgraphsdk.SignInsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.AuditLogs().SignIns().GetWithRequestConfigurationAndResponseHandler(options, nil)


```