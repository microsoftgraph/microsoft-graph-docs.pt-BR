---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9d0bd99c425b3885be99f1381137c223f5aa16a8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082356"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedGroupSource()
group := msgraphsdk.NewGroup()
requestBody.SetGroup(group)
mail := "SecretGroup@contoso.com"
group.SetMail(&mail)
includedSources := "mailbox, site"
requestBody.SetIncludedSources(&includedSources)
options := &msgraphsdk.UnifiedGroupSourcesRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
custodianId := "custodian-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UnifiedGroupSources().Post(options)


```