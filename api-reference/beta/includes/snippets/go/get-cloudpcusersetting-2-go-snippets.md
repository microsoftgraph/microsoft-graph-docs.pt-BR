---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a890fcc06252f402d951c85b2872a1574a669c45
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975627"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.CloudPcUserSettingRequestBuilderGetQueryParameters{
    Expand: "assignments",
}
options := &msgraphsdk.CloudPcUserSettingRequestBuilderGetOptions{
    Q: requestParameters,
}
cloudPcUserSettingId := "cloudPcUserSetting-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().UserSettingsById(&cloudPcUserSettingId).Get(options)


```