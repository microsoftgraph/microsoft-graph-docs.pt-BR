---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d65d6559e192dcd501edab407210e3a60a6fe414
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033583"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

setId := "set-id"
result, err := graphClient.TermStore().SetsById(&setId).Children().Get(options)


```