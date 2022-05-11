---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3a695dece1fb716333044465920107e32364358
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323007"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTaskFolder()
name := "Cooking"
requestBody.SetName(&name)
outlookTaskGroupId := "outlookTaskGroup-id"
result, err := graphClient.Me().Outlook().TaskGroupsById(&outlookTaskGroupId).TaskFolders().Post(requestBody)


```