---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ad78a2768c18f4768a920f21819767d6278e478
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028822"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewContactFolder()
parentFolderId := "parentFolderId-value"
requestBody.SetParentFolderId(&parentFolderId)
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ContactFolderRequestBuilderPatchOptions{
    Body: requestBody,
}
contactFolderId := "contactFolder-id"
graphClient.Me().ContactFoldersById(&contactFolderId).Patch(options)


```