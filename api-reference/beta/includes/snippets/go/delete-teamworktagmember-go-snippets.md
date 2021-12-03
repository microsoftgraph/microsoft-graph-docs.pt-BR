---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b462183ccb78528f63a473cc749fc439905a54a9
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286922"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
teamworkTagId := "teamworkTag-id"
teamworkTagMemberId := "teamworkTagMember-id"
graphClient.TeamsById(&teamId).TagsById(&teamworkTagId).MembersById(&teamworkTagMemberId).Delete(nil)


```