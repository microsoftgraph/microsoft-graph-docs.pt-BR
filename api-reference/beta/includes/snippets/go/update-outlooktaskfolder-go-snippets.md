---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb1730e5fa39061cb9a7f4bcfbbe638b241e6d0f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322689"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTaskFolder()
name := "Charity work"
requestBody.SetName(&name)
outlookTaskFolderId := "outlookTaskFolder-id"
graphClient.Me().Outlook().TaskFoldersById(&outlookTaskFolderId).Patch(requestBody)


```