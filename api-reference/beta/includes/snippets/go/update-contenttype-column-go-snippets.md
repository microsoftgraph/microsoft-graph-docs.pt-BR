---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce1d38caae41d056f82b817804a5f31a43b0672f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410541"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewColumnDefinition()
required := true
requestBody.SetRequired(&required)
hidden := false
requestBody.SetHidden(&hidden)
propagateChanges := false
requestBody.SetPropagateChanges(&propagateChanges)
options := &msgraphsdk.ColumnDefinitionRequestBuilderPatchOptions{
    Body: requestBody,
}
siteId := "site-id"
contentTypeId := "contentType-id"
columnDefinitionId := "columnDefinition-id"
result, err := graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).ColumnsById(&columnDefinitionId).Patch(options)


```