---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee8549eb38d7e581e55fc5aca2b5566b3f9d438f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977600"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

setId := "set-id"
result, err := graphClient.TermStore().SetsById(&setId).Relations().Get(options)


```