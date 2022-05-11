---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 357f6101131b2f28cb6107e0101be07ae4704deb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325050"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContactFolder()
parentFolderId := "parentFolderId-value"
requestBody.SetParentFolderId(&parentFolderId)
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
contactFolderId := "contactFolder-id"
graphClient.Me().ContactFoldersById(&contactFolderId).Patch(requestBody)


```