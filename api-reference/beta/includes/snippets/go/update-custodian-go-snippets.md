---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 451a701422c6ec5925db459497be14e2d7b45991
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120899"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCustodian()
applyHoldToSources := "false"
requestBody.SetApplyHoldToSources(&applyHoldToSources)
options := &msgraphsdk.CustodianRequestBuilderPatchOptions{
    Body: requestBody,
}
caseId := "case-id"
custodianId := "custodian-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).Patch(options)


```