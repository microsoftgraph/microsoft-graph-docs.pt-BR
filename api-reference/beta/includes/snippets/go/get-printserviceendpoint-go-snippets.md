---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2ad4d5f6ae754fe55b5fdf3348a5b50e1d437b0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101140"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printServiceId := "printService-id"
printServiceEndpointId := "printServiceEndpoint-id"
result, err := graphClient.Print().ServicesById(&printServiceId).EndpointsById(&printServiceEndpointId).Get(options)


```