---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c80b5423bbbd8467a3017343693d137d845b98dc
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286520"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
schedulingGroupId := "schedulingGroup-id"
graphClient.TeamsById(&teamId).Schedule().SchedulingGroupsById(&schedulingGroupId).Delete(nil)


```