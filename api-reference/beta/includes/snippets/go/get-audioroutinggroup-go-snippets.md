---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2dd0d883d907c5a8d46999d62d73401eaa9525e4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982459"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

callId := "call-id"
audioRoutingGroupId := "audioRoutingGroup-id"
result, err := graphClient.Communications().CallsById(&callId).AudioRoutingGroupsById(&audioRoutingGroupId).Get(options)


```