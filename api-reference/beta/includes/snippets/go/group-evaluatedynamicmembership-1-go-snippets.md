---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37c87a92aee79d7481f58968457d0c107ea7d752
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325671"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMemberIdRequestBody()
memberId := "319b41e8-d9e4-42f8-bdc9-741113f48b33"
requestBody.SetMemberId(&memberId)
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).EvaluateDynamicMembership(group-id).Post(requestBody)


```