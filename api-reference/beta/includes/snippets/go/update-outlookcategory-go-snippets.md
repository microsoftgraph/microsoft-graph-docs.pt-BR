---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3446273925243ce9fe4e638d46dfaed8575e1e0e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090474"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookCategory()
color := "preset15"
requestBody.SetColor(&color)
options := &msgraphsdk.OutlookCategoryRequestBuilderPatchOptions{
    Body: requestBody,
}
outlookCategoryId := "outlookCategory-id"
graphClient.Me().Outlook().MasterCategoriesById(&outlookCategoryId).Patch(options)


```