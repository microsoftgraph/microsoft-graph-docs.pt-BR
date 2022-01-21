---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce0ac8a28f0a1f3bb79130af878721aac8343bd6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127388"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMailFolder()
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.MailFolderRequestBuilderPatchOptions{
    Body: requestBody,
}
mailFolderId := "mailFolder-id"
graphClient.Me().MailFoldersById(&mailFolderId).Patch(options)


```