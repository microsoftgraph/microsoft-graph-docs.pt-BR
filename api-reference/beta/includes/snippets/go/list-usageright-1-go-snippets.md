---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93c5cf66cbf12f4199f02daf0e7d721a40a3276f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015719"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).UsageRights().Get(options)


```