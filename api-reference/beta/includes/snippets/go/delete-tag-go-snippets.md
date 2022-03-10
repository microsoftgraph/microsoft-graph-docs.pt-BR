---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62d8e00f477b9c32b98b51bf3ce9a9fbb5336b85
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411492"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TagRequestBuilderDeleteQueryParameters{
    Forcedelete: true,
}
options := &msgraphsdk.TagRequestBuilderDeleteOptions{
    Q: requestParameters,
}
caseId := "case-id"
tagId := "tag-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).TagsById(&tagId).Delete(options)


```