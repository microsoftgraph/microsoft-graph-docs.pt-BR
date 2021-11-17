---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df1cd4eac176484f8786ed388ade59fa47995101
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989550"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

tiIndicatorId := "tiIndicator-id"
result, err := graphClient.Security().TiIndicatorsById(&tiIndicatorId).Get(options)


```