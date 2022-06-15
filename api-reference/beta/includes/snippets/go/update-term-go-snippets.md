---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f5d916618067c98c41f933a8210749a5415be733
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093463"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTerm()
requestBody.SetLabels( []LocalizedLabel {
    msgraphsdk.NewLocalizedLabel(),
name := "changedLabel"
    SetName(&name)
languageTag := "en-US"
    SetLanguageTag(&languageTag)
isDefault := true
    SetIsDefault(&isDefault)
}
setId := "set-id"
termId := "term-id"
graphClient.TermStore().SetsById(&setId).TermsById(&termId).Patch(requestBody)


```