---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c8278dc83c905d848260e0b3ca3a67db7c4d4ee
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324729"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCustodian()
email := "AdeleV@contoso.com"
requestBody.SetEmail(&email)
applyHoldToSources := "true"
requestBody.SetApplyHoldToSources(&applyHoldToSources)
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).Custodians().Post(requestBody)


```