---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58ef193358ac402a29025633da59c79a998c55f9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324252"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
teamworkTagId := "teamworkTag-id"
teamworkTagMemberId := "teamworkTagMember-id"
graphClient.TeamsById(&teamId).TagsById(&teamworkTagId).MembersById(&teamworkTagMemberId).Delete()


```