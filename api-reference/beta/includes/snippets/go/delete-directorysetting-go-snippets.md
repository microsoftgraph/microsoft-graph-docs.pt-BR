---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 149df2e085f7c7b4eac45e4df89ea9fbd747c953
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324424"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directorySettingId := "directorySetting-id"
graphClient.SettingsById(&directorySettingId).Delete()


```