---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 256057ea8f9a38a67d9b94147d31702737f17244
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394611"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroupSetting()
requestBody.SetValues( []SettingValue {
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "AllowToAddGuests",
        "value": "true",
    }
}
options := &msgraphsdk.GroupSettingRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
groupSettingId := "groupSetting-id"
result, err := graphClient.GroupsById(&groupId).SettingsById(&groupSettingId).Patch(options)


```