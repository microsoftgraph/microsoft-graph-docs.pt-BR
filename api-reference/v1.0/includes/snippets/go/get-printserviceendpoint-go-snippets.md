---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13ea64715255bbf6c58ac996511f6af8b4c1ce0e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992540"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printServiceId := "printService-id"
printServiceEndpointId := "printServiceEndpoint-id"
result, err := graphClient.Print().ServicesById(&printServiceId).EndpointsById(&printServiceEndpointId).Get(options)


```