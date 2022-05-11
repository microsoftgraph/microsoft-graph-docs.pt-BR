---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28f4441a2e2ea48e9f23d5ef1f94ad5335f6ebae
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323928"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userActivityId := "userActivity-id"
graphClient.Me().ActivitiesById(&userActivityId).Delete()


```