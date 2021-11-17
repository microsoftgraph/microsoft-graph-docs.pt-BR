---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36444e67594b0ff1f8139575457a415656c9ab49
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982775"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

applicationSignInDetailedSummaryId := "applicationSignInDetailedSummary-id"
result, err := graphClient.Reports().ApplicationSignInDetailedSummaryById(&applicationSignInDetailedSummaryId).Get(options)


```