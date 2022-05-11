---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7a39cd9e0045b917b286735a57a086d3832546a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323563"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCustodian()
applyHoldToSources := "false"
requestBody.SetApplyHoldToSources(&applyHoldToSources)
caseId := "case-id"
custodianId := "custodian-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).Patch(requestBody)


```