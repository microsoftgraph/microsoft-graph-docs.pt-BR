---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dad37a3dde9df3b626878a2e3554d3d9d510b3c1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027057"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
conversationMemberId := "conversationMember-id"
result, err := graphClient.TeamsById(&teamId).MembersById(&conversationMemberId).Get(options)


```