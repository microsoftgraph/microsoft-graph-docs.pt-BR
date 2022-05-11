---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a37e05eba98381edc5dfcd7fa0dd4d68da6304ac
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325052"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcUserSettingId := "cloudPcUserSetting-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().UserSettingsById(&cloudPcUserSettingId).Get()


```