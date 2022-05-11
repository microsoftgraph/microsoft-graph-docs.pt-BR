---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98ca58b60b42f129a0d2b505e89f72d44d78f304
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323900"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDirectorySetting()
requestBody.SetValues( []SettingValue {
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "CustomBlockedWordsList",
        "value": "Contoso",
    }
}
directorySettingId := "directorySetting-id"
graphClient.SettingsById(&directorySettingId).Patch(requestBody)


```