---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afab8908a20f934bd067f6e0bc7ee4c153c68f56
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324244"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Teamwork().InstalledApps().Get()


```