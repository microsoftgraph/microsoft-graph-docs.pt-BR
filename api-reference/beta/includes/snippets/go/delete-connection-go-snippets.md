---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0938fbb4426062ec2d6c4dcbcd5ba35a23baef9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981508"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

externalConnectionId := "externalConnection-id"
graphClient.External().ConnectionsById(&externalConnectionId).Delete(options)


```