---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2261132abdb2d128f6c2ee4bade8e98de18de15
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324046"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewLinkedResource()
webUrl := "https://microsoft.com"
requestBody.SetWebUrl(&webUrl)
applicationName := "Microsoft"
requestBody.SetApplicationName(&applicationName)
displayName := "Microsoft"
requestBody.SetDisplayName(&displayName)
externalId := "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
requestBody.SetExternalId(&externalId)
todoTaskListId := "todoTaskList-id"
todoTaskId := "todoTask-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).LinkedResources().Post(requestBody)


```