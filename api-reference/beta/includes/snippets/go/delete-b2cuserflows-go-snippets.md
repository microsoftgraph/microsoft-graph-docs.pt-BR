---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d13992d5ba0444ba80625457e500cde18e724bc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60999968"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).Delete(options)


```