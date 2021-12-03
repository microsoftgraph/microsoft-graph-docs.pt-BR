---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60d59fb54c64d2cc15d1aa49648c0aa72e408946
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286143"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcUserSettingId := "cloudPcUserSetting-id"
graphClient.DeviceManagement().VirtualEndpoint().UserSettingsById(&cloudPcUserSettingId).Delete(nil)


```