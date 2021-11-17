---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d48f176a2a87744aa96e171679ca745b6b210bb9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001626"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
timeOffId := "timeOff-id"
graphClient.TeamsById(&teamId).Schedule().TimesOffById(&timeOffId).Delete(options)


```