---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b79e2cf70ab989d78ec2269d108dfe740885b67b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410885"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
teamworkTagId := "teamworkTag-id"
teamworkTagMemberId := "teamworkTagMember-id"
result, err := graphClient.TeamsById(&teamId).TagsById(&teamworkTagId).MembersById(&teamworkTagMemberId).Delete(nil)


```