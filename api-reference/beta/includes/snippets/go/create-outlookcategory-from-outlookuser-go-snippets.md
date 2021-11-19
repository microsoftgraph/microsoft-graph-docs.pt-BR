---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5820672ca5e3c1b08764871b44a6f976d655cc03
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085161"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookCategory()
displayName := "Project expenses"
requestBody.SetDisplayName(&displayName)
color := "preset9"
requestBody.SetColor(&color)
options := &msgraphsdk.MasterCategoriesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Outlook().MasterCategories().Post(options)


```