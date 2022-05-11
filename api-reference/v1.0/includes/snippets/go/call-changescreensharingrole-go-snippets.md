---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6955f15f8bea46d1cd6848ac6df54652ad50ac98
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322954"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewRoleRequestBody()
role := "viewer"
requestBody.SetRole(&role)
callId := "call-id"
graphClient.Communications().CallsById(&callId).ChangeScreenSharingRole(call-id).Post(requestBody)


```