---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88812d07283d311c221e6ffcb0cea76d83403d8c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323062"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupSettingId := "groupSetting-id"
graphClient.GroupSettingsById(&groupSettingId).Delete()


```