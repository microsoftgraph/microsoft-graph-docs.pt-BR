---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0dd8c82a53e24ad8f1a9cfc5cd5defd9c843b60a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287075"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printServiceId := "printService-id"
printServiceEndpointId := "printServiceEndpoint-id"
result, err := graphClient.Print().ServicesById(&printServiceId).EndpointsById(&printServiceEndpointId).Get(nil)


```