---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5e919bdd2a0d1b576b857520a0247260e662502
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324590"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
endpointId := "endpoint-id"
result, err := graphClient.GroupsById(&groupId).EndpointsById(&endpointId).Get()


```