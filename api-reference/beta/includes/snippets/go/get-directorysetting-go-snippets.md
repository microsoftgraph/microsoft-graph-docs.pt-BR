---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 640d8b7490a4550000fa15c71e82d5d7d90c71b5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090917"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directorySettingId := "directorySetting-id"
result, err := graphClient.SettingsById(&directorySettingId).Get(options)


```