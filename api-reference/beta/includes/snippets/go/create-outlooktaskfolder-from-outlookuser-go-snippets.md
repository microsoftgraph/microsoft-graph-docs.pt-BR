---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66005e1276732ddf3f4081b9ec68e5361d8f459d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325610"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTaskFolder()
name := "Volunteer"
requestBody.SetName(&name)
result, err := graphClient.Me().Outlook().TaskFolders().Post(requestBody)


```