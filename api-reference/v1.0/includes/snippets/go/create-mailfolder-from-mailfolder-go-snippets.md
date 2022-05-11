---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 395d233be2c49d42c9d3eb2fb45fecb053d258ee
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323271"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMailFolder()
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
isHidden := true
requestBody.SetIsHidden(&isHidden)
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).ChildFolders().Post(requestBody)


```