---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2ef457f2b54b98757b48814266dfd21b9627ed22
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325141"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMailFolder()
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
mailFolderId := "mailFolder-id"
graphClient.Me().MailFoldersById(&mailFolderId).Patch(requestBody)


```