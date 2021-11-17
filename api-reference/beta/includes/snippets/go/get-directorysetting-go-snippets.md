---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 422297f70233daae3afdf1b49b624e97c11d5d7d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982123"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

directorySettingId := "directorySetting-id"
result, err := graphClient.SettingsById(&directorySettingId).Get(options)


```