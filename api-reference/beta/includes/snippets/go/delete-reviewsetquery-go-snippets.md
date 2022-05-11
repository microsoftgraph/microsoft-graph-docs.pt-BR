---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 121de9dbb3fe47c8476fcf3749b9ab9811c01580
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322890"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
reviewSetId := "reviewSet-id"
reviewSetQueryId := "reviewSetQuery-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).QueriesById(&reviewSetQueryId).Delete()


```