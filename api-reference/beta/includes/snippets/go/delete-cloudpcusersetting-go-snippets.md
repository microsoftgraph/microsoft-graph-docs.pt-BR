---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c2e57d1b260d0be328493abfad1605533637a58
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323909"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcUserSettingId := "cloudPcUserSetting-id"
graphClient.DeviceManagement().VirtualEndpoint().UserSettingsById(&cloudPcUserSettingId).Delete()


```