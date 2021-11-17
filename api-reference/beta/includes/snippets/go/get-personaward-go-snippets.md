---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91db08dc55fdae423e10472285bc835e4f3fe542
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997846"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

personAwardId := "personAward-id"
result, err := graphClient.Me().Profile().AwardsById(&personAwardId).Get(options)


```