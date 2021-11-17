---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0b89e01af9686e8ca3a28edc839104853da8ff70
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018714"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

caseId := "case-id"
reviewSetId := "reviewSet-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).Queries().Get(options)


```