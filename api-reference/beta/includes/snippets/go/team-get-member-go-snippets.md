---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4f1e04e131c26c8ad682df22e53474ca82aeffb
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287181"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
conversationMemberId := "conversationMember-id"
result, err := graphClient.TeamsById(&teamId).MembersById(&conversationMemberId).Get(nil)


```