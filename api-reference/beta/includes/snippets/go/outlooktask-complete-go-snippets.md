---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3155206cb269f4220a9eb48acebdc98fcc3a0bc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323112"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.CompleteRequestBuilderPostRequestConfiguration{
    Headers: headers,
}
outlookTaskId := "outlookTask-id"
result, err := graphClient.Me().Outlook().TasksById(&outlookTaskId).Complete(outlookTask-id).PostWithRequestConfigurationAndResponseHandler(options, nil)


```