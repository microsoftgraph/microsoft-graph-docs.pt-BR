---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da145a38fcb9365e2f9e0c1296a3d3992467ba29
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031153"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).Get(options)


```