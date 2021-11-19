---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd8a633c285899dcf22fe5f6985a45af85da70c0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085392"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
legalHoldId := "legalHold-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).LegalHoldsById(&legalHoldId).SiteSources().Get(options)


```