---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb3fd6e51a347a0da40bdc6408319f67635e0f36
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022564"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewCloudPcUserSetting()
displayName := "Example"
requestBody.SetDisplayName(&displayName)
selfServiceEnabled := true
requestBody.SetSelfServiceEnabled(&selfServiceEnabled)
localAdminEnabled := false
requestBody.SetLocalAdminEnabled(&localAdminEnabled)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcUserSetting",
}
options := &msgraphsdk.CloudPcUserSettingRequestBuilderPatchOptions{
    Body: requestBody,
}
cloudPcUserSettingId := "cloudPcUserSetting-id"
graphClient.DeviceManagement().VirtualEndpoint().UserSettingsById(&cloudPcUserSettingId).Patch(options)


```